<template>
    <div class="flex flex-col max-w-[410px] ">
        <div class="">
            <img :src="card.image" alt="ServiceIcon" class="-mt-5   w-[410px] h-[256px]" />
        </div>
        
        <div class="flex flex-col mt-2">
            <span class="text-[#343f52] text-[22px] text-left">{{card.title }}</span>
            <div class="flex flex-row mt-5"> 
                <span class="text-[#aab0bc] flex">
                    <img src="../../../assets/icons/date.svg" class="mr-2"/>
                    {{ card.date }}
                </span>
                <span class="text-[#aab0bc] ml-5 flex">
                    <img src="../../../assets/icons/ites.svg" class="mr-2"/>
                    {{ card.task }}</span>
            </div>

        </div>

        
    </div>
</template>
<script setup>
const props =defineProps({
    card: {
    type: Array, 
    required: true,
  },

})

</script>
<style>
    
</style>