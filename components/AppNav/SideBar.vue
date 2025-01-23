<template>
  <aside class="w-full h-[100%] p-4 bg-[#FEFEFE] ml-4">
    <nav class="flex flex-col gap-4 justify-center items-center mt-[100px]">
      <ul class="space-y-4">
        <li v-for="(link, index) in links" :key="index">
          <a
            :href="'#' + link.id"
            @click.prevent="scrollToSection(link.id)"
            :class="[
              'text-gray-600 text-[20px] cursor-pointer',
              activeSection === link.id
                ? 'text-blue-500 underline'
                : 'hover:text-blue-500 hover:underline',
            ]"
          >
            {{ link.name }}
          </a>
        </li>
      </ul>
    </nav>
  </aside>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const activeSection = ref(null);

const links = [
  { id: "term", name: "Terms & Conditions" },
  { id: "privacy-policy", name: "Privacy Policy" },
  { id: "user-policy", name: "User Policy" },
  { id: "copyright", name: "Copyrights" },
  { id: "Cookies", name: "Cookies" },
  { id: "account-billing", name: "Account & Billing" },
];

const scrollToSection = (id) => {
  document.getElementById(id).scrollIntoView({ behavior: "smooth" });
};

const observeSections = () => {
  const observer = new IntersectionObserver(
    (entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          activeSection.value = entry.target.id;
        }
      });
    },
    { root: null, threshold: 0.6 }
  );

  links.forEach((link) => {
    const section = document.getElementById(link.id);
    if (section) {
      observer.observe(section);
    }
  });

  return observer;
};

onMounted(() => {
  const observer = observeSections();
  onUnmounted(() => observer.disconnect());
});
</script>
