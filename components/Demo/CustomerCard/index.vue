<template>
  <div
    class="w-full md:w-1/2 lg:w-1/3 h-[300px] md:h-[400px] lg:h-[450px] border rounded-xl grid lg:grid-cols-4"
  >
    <div class="p-5">
      <p class="text-[21px] text-gray-400 mb-3">“{{ text }}”</p>
      <div class="flex items-center gap-6">
        <img
          :src="img"
          alt="testimonial image"
          class="!rounded-[50%] !w-[3.8rem] md:!w-16 lg:!w-20"
        />
        <div class="flex flex-col gap-2">
          <div class="font-sans font-bold text-[23px] md:text-[28px] mt-4">
            {{ name }}
          </div>
          <div
            class="text-gray-400 text-[21px] font-sans font-semibold md:text-[25px]"
          >
            {{ title }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TestimonialCard",
  props: {
    text: {
      type: String,
      required: true,
    },
    img: {
      type: String,
      required: true,
    },
    name: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
/* Add any scoped styles if needed */
</style>
