<template>
  <div class="relative w-full h-[500px]">
    <div class="parallax-container">
      <Parallax :strength="0.5">
        <iframe
          src="https://www.youtube.com/embed/CQEPHM_tuYw?si=qRtDnP7ZzqrJVJRm"
          frameborder="0"
          class="w-full h-[500px] absolute  z-6 opacity-45 "
        >
        </iframe>
        <div
          class="absolute text-white text-center mt-[250px] font-semibold text-[20px]"
        >
          Find out everything you need to know about creating a business process model.
        </div>
      </Parallax>
    </div>
  </div>
</template>

<script>
import { Parallax } from 'vue-parallaxy';


export default {
  components: { Parallax },
};
</script>

<style scoped>
.parallax-container {
  height: 500px;
  overflow: hidden;
  position: relative;
}

</style>