<script setup>
import NavBar from './NavBar.vue'; // Correctly import the NavBar component
</script>

<template>
  <NavBar /> <!-- Use NavBar component here -->
</template>


<template>
  <div>
    <div class="flex flex-col min-h-screen">
      <NavBar />
      <!-- <slot /> -->
      <!-- <FooterPage /> -->
    </div>
  </div>
</template>
