<template>
  <div class="flex flex-row m-5 w-full">
    <img :src="card.image" alt="ServiceIcon" class="max-w-14 max-h-14" />
    <div class="flex flex-col ml-[25.5px]">
      <h1 class="text-[20px] font-bold text-[#353F53] mb-2 ">{{ card.title }}</h1>
      <span
        class="text-base text-gray-500 text-[16px] max-w-md leading-relaxed md:leading-7 lg:leading-8"
      >
        {{ card.description }}
      </span>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  card: {
    type: Array, 
    required: true,
  },
});
</script>

<style scoped>

</style>
