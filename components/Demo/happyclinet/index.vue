<template>
  <div>
    <section class="wrapper bg-white">
      <div class="container pt-20 xl:pt-28 pb-16 xl:pb-20">
        <h2 class="text-3xl font-bold text-center mb-3">Happy Customers</h2>
        <p class="text-lg font-medium text-center mb-6">
          Customer satisfaction is our major goal. See what our customers are
          saying about us.
        </p>

        <div
          class="relative ml-[445px] w-[400px] h-[340px] border rounded-xl shadow-xl border-gray-400 justify-center items-center"
        >
          <div class="flex overflow-hidden justify-center items-center">
            <div
              class="flex transition-transform duration-500 w-[350px] h-[300px]"
              :style="{ transform: `translateX(-${currentSlide * 100}%)` }"
            >
              <div
                class="min-w-full flex flex-col items-center p-6 text-center"
                v-for="(item, index) in data"
                :key="index"
              >
                <img
                  :src="item.img"
                  :alt="item.name"
                  class="w-24 h-24 rounded-full mb-4 object-cover"
                />
                <h3 class="text-xl font-semibold">{{ item.name }}</h3>
                <p class="text-gray-500 text-sm mb-2">{{ item.title }}</p>
                <p class="text-gray-700">{{ item.text }}</p>
              </div>
            </div>
          </div>

          <div class="flex justify-center mt-16">
            <span
              v-for="(item, index) in data"
              :key="index"
              class="w-3 h-3 rounded-full mx-1 cursor-pointer"
              :class="index === currentSlide ? 'bg-blue-500' : 'bg-gray-300'"
              @click="setSlide(index)"
            ></span>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import { ref } from "vue";

const data = [
  {
    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis lacus vel augue.",
    img: "https://sandbox-tailwind-template.netlify.app/assets/img/avatars/te3.jpg",
    name: "Nikolas Brooten",
    title: "Sales Manager",
  },
  {
    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis lacus vel augue.",
    img: "https://sandbox-tailwind-template.netlify.app/assets/img/avatars/te2.jpg",
    name: "Emily Wilson",
    title: "Product Manager",
  },
  {
    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis lacus vel augue.",
    img: "https://sandbox-tailwind-template.netlify.app/assets/img/avatars/te1.jpg",
    name: "John Doe",
    title: "Software Engineer",
  },
  {
    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis lacus vel augue.",
    img: "https://sandbox-tailwind-template.netlify.app/assets/img/avatars/te4.jpg",
    name: "Sophia Loren",
    title: "Designer",
  },
];

const currentSlide = ref(0);

const prevSlide = () => {
  currentSlide.value = (currentSlide.value - 1 + data.length) % data.length;
};

const nextSlide = () => {
  currentSlide.value = (currentSlide.value + 1) % data.length;
};

const setSlide = (index) => {
  currentSlide.value = index;
};
</script>

<style scoped>
.wrapper {
  background-color: #ffffff;
}

.container {
  margin: auto;
  max-width: 1200px;
}

button {
  z-index: 10;
}

img {
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
}
</style>
