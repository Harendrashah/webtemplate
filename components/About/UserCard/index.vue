<template>
  <div class="w-[292px] h-[400px] border border-gray-200 rounded-md p-[40px] mt-[20px]">
    <!-- Profile -->
    <img
      :src="profileImage"
      alt="Profile Picture"
      class="w-[100px] h-[100px] rounded-full object-cover object-top"
    />
    <div class="flex flex-col gap-5 mb-[20px]">
      <span class="mt-[20px] text-[19px] font-bold">{{ name }}</span>
      <span class="text-gray-500">{{ title }}</span>
      <span class="text-gray-600">{{description}}.</span>
    </div>
    <!-- Icons (Static) -->
    <div class="flex gap-4">
      <img src="../../../assets/icons/facebook.svg" alt="Facebook" />
      <img src="../../../assets/icons/twitter.svg" alt="Twitter" />
      <img src="../../../assets/icons/dribble.svg" alt="Dribbble" />
    </div>
  </div>
</template>

<script setup>
defineProps({
  name: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  profileImage: {
    type: String,
    required: true,
  },
  description:{
    type:String,
    required:true,
  }
});
</script>
