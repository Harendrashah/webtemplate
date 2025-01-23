<template>
  <div class="relative">
    <div class="relative bg-slate-300">
      <img
        src="../../../assets/images/bgdemo.jpg"
        class="relative hidden lg:block bg-gray-200"
        alt="background"
      />

        <div class=" relative md:absolute flex flex-col mt-[50px] justify-center items-center top-0">
          <div
            class="flex flex-col md:justify-center ml-10 xl:mt-20  xl:ml-20"
          >
            <img src="@/assets/icons/webringsoln.svg" alt="webringsoln" class="size-full font-bold "/>
            <img
              src="@/assets/icons/des.svg"
              class="mt-5"
              alt="webringsoln"
            />


            
            <div class="mt-[35.2px]">
             <nuxt-link to="/about">
    <button class="bg-[#343F52] text-white p-1 mb-2 items-center md:p-5 rounded-md">
      Read more
    </button>
  </nuxt-link>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>
<script setup>

</script>
<style>
    
</style>