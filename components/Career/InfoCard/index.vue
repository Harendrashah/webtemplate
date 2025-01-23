<template>
  <div class="flex m-5 p-4 bg-white rounded-lg shadow-md items-center w-full transform transition duration-300 hover:translate-y-[-5px] hover:shadow-lg">
    <!-- Profile Image and Name -->
    <div class="flex items-center space-x-4 w-1/4">
      <img
        src="@/assets/images/g14.jpg"
        class="w-[45px] h-[45px] rounded-full"
        alt="Profile Image"
      />
      <span class="text-lg font-medium text-gray-800">{{ card.name }}</span>
    </div>

    <!-- Position Type -->
    <div class="flex items-center w-1/4 text-gray-700">
      <img
        src="../../../assets/icons/time.svg"
        alt="Time Icon"
        class="w-5 h-5 mr-2"
      />
      <span class="text-lg">{{ card.time }}</span>
    </div>

    <!-- Location -->
    <div class="flex items-center w-1/4 text-gray-700">
      <img
        src="../../../assets/icons/arror.svg"
        alt="Location Icon"
        class="w-5 h-5 mr-2"
      />
      <span class="text-lg">{{ card.location }}</span>
    </div>

    <!-- Action Icon -->
    <div class="text-blue-500 text-lg w-1/4 text-center">
      <span class="cursor-pointer text-xl"><strong>...</strong></span>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  card: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped></style>
