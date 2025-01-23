<template>
  <div class="bg-white rounded-lg shadow overflow-hidden">
    <img :src="image" alt="Blog Image" class="w-full h-64 object-cover" />
    <div class="p-6">
      <p class="text-sm text-blue-500 font-medium">{{ category }}</p>
      <h2 class="text-xl font-bold text-gray-800 mt-2">{{ title }}</h2>
      <p class="text-gray-600 mt-4">{{ excerpt }}</p>
      <div class="flex justify-between items-center mt-6 text-gray-500 text-sm">
        <span>{{ date }}</span>
        <span>{{ comments }} comments</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image: String,
    title: String,
    excerpt: String,
    date: String,
    category: String,
    comments: Number,
  },
};
</script>
