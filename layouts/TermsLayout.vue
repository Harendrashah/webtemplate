<template>
  <div class="flex bg-[#FEFEFE] min-h-screen">
    <div class="w-[20%] sticky top-0 self-start">
      <SideBar />
    </div>
    <div class="ml-[10%] w-[80%]">
      <slot />
    </div>
  </div>
</template>

<script setup>
import SideBar from "~/components/AppNav/SideBar.vue";
</script>
