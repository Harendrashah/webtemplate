<template>
  <div
    :class="[
      'sticky top-0 z-50 bg-white transition-transform duration-300',
      navColor,
      isNavbarVisible ? 'translate-y-0' : '-translate-y-full',
    ]"
  >
    <header>
      <div :class="['flex justify-between items-center p-2', navColor]">
        <div class="ml-[150px]">
          <img
            src="https://yajtechnologies.com/assets/newtheme/img/logo.png"
            alt="Logo"
            class="w-[110px] h-[50px]"
          />
        </div>

        <div class="hidden md:flex justify-center items-center gap-9">
          <NuxtLink to="/">
            <div class="font-sans font-semibold text-[18px] text-[#515a69]">
              Home
            </div>
          </NuxtLink>
          <NuxtLink to="/service">
            <div class="font-sans font-semibold text-[18px] text-[#515a69]">
              Services
            </div>
          </NuxtLink>
          <NuxtLink to="/About">
            <div class="font-sans font-semibold text-[18px] text-[#515a69]">
              About Us
            </div>
          </NuxtLink>
          <NuxtLink to="/blogs">
            <div class="font-sans font-semibold text-[18px] text-[#515a69]">
              Blogs
            </div>
          </NuxtLink>
          <NuxtLink to="/project">
            <div class="font-sans font-semibold text-[18px] text-[#515a69]">
              Projects
            </div>
          </NuxtLink>
          <NuxtLink to="/carrer">
            <div class="font-sans font-semibold text-[18px] text-[#515a69]">
              Career
            </div>
          </NuxtLink>
        </div>

        <div class="hidden md:flex justify-end items-center ml-[145px]">
          <NuxtLink to="/Contactus">
            <div
              class="bg-blue-500 flex justify-center items-center text-[18px] font-semibold font-sans rounded-full text-white w-[105px] h-[40px] mr-[50px]"
            >
              Contact Us
            </div>
          </NuxtLink>
        </div>

        <div class="md:hidden flex items-center" @click="toggleMenu">
          <button class="text-black">
            <span v-if="!isMenuOpen">☰</span>
            <span v-else>×</span>
          </button>
        </div>
      </div>

      <div
        v-show="isMenuOpen"
        class="md:hidden flex flex-col items-center gap-4 mt-4"
      >
        <NuxtLink to="/demo" @click="toggleMenu">
          <div class="font-sans font-semibold text-[18px] text-[#515a69]">
            Home
          </div>
        </NuxtLink>
        <NuxtLink to="/service" @click="toggleMenu">
          <div class="font-sans font-semibold text-[18px] text-[#515a69]">
            Services
          </div>
        </NuxtLink>
        <NuxtLink to="/About" @click="toggleMenu">
          <div class="font-sans font-semibold text-[18px] text-[#515a69]">
            About
          </div>
        </NuxtLink>
        <NuxtLink to="/blogs" @click="toggleMenu">
          <div class="font-sans font-semibold text-[18px] text-[#515a69]">
            Blogs
          </div>
        </NuxtLink>
        <NuxtLink to="/project" @click="toggleMenu">
          <div class="font-sans font-semibold text-[18px] text-[#515a69]">
            Projects
          </div>
        </NuxtLink>
        <NuxtLink to="/carrer" @click="toggleMenu">
          <div class="font-sans font-semibold text-[18px] text-[#515a69]">
            Career
          </div>
        </NuxtLink>
        <NuxtLink to="/Contactus" @click="toggleMenu">
          <div
            class="bg-blue-500 flex justify-center items-center text-[18px] font-bold font-sans rounded-full text-white w-[130px] h-[60px]"
          >
            Contact Us
          </div>
        </NuxtLink>
      </div>
    </header>
  </div>
</template>

<script setup>

import { ref, onMounted, onBeforeUnmount, computed } from 'vue';  // Add missing imports
import { useRoute } from 'vue-router';

const route = useRoute();

// navbar change color if path is /carrer
const navColor = computed(() => {
  if (route.path === '/carrer'|| route.path === '/blogs' || route.path === '/service') {
    return 'bg-[#EDF2FC]';
  }
  return '';
});

const isNavbarVisible = ref(true);
const lastScrollY = ref(0);
const hideTimeout = ref(null);

const isMenuOpen = ref(false);

// Toggle the mobile menu visibility
const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};

// Handle scroll behavior
const handleScroll = () => {
  const currentScrollY = window.scrollY;

  if (currentScrollY > lastScrollY.value) {
    isNavbarVisible.value = false;

    if (hideTimeout.value) clearTimeout(hideTimeout.value);

    hideTimeout.value = setTimeout(() => {
      isNavbarVisible.value = true;
    }, 30);
  } else {
    isNavbarVisible.value = true;

    if (hideTimeout.value) clearTimeout(hideTimeout.value);
  }

  lastScrollY.value = currentScrollY;
};

// Attach scroll event listener
onMounted(() => {
  window.addEventListener('scroll', handleScroll);
});

// Clean up the event listener on unmount
onBeforeUnmount(() => {
  window.removeEventListener('scroll', handleScroll);
  if (hideTimeout.value) clearTimeout(hideTimeout.value);
});
</script>

<style scoped>
.sticky {
  will-change: transform;
}
</style>
