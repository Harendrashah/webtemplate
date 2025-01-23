<template>
  <div>
    <div class="p-6 flex">
      <div
        class="xl:w-4/12 lg:w-4/12 w-full flex-[0_0_auto] xl:px-[35px] lg:px-[20px] px-[15px] max-w-full mt-[30px]"
      >
        <h2
          class="text-[calc(1.305rem_+_0.66vw)] font-bold xl:text-[2rem] leading-[1.3] xl:!mt-32 lg:!mt-32 !mb-3"
        >
          Our Pricing
        </h2>
        <p class="lead !text-[1.2rem] text-gray-700 !leading-[1.6] font-medium">
          We offer
          <span
            class="relative z-[2] whitespace-nowrap after:content-[''] after:block after:absolute after:w-[102.5%] after:h-[30%] after:left-[-1.5%] after:z-[-1] after:transition-all after:duration-[0.2s] after:ease-in-out after:mt-0 after:rounded-[5rem] after:bottom-[9%] motion-reduce:after:transition-none after:bg-[rgba(63,120,224,.12)]"
            >great prices</span
          >, premium and quality products for your business.
        </p>
        <p class="text-[1.1rem] mt-3">
          Enjoy a
          <a href="#" class="hover:underline text-blue-500"
            >free 30-day trial</a
          >
          and experience the full service. No credit card required!
        </p>
        <p
          class="!w-[140px] mt-4 text-center  flex items-center justify-center font-bold !h-[40px] bg-blue-500 rounded-full text-white"
        >
          See All Prices
        </p>
      </div>
      <div>
        <div class="flex items-center justify-center mt-12 mb-5 ml-[487px]">
          <p class="text-lg font-medium text-gray-600 pr-4">Monthly</p>
          <div
            class="relative w-12 h-6 bg-gray-300 p-1 rounded-full cursor-pointer"
            @click="togglePricing"
          >
            <div
              class="absolute w-5 h-5 bg-blue-500 rounded-full transition-all"
              :class="{ 'left-1': isMonthly, 'right-1': !isMonthly }"
            ></div>
          </div>
          <p class="text-lg font-medium text-gray-600 pl-4">
            Yearly <span class="text-red-500">(Save 30%)</span>
          </p>
        </div>

        <div class="relative ml-[170px]">
          <transition name="fade" mode="out-in">
            <div
              v-if="isMonthly"
              key="monthly"
              class="flex justify-center gap-6"
            >
              <div
                class="w-80 h-96 border p-6 rounded-xl shadow-md bg-white flex flex-col justify-center items-center"
              >
                <h4 class="text-2xl font-bold mb-4">Basic Plan</h4>
                <p class="text-gray-500 text-lg mb-6">$19 / mo</p>
                <ul class="text-gray-600 space-y-3 mb-6">
                  <li>5 Projects</li>
                  <li>100K API Access</li>
                  <li>200MB Storage</li>
                  <li>Weekly Reports</li>
                  <li>24/7 Support</li>
                </ul>
                <button class="bg-blue-500 text-white px-6 py-2 rounded-full">
                  Choose Plan
                </button>
              </div>

              <div
                class="w-80 h-96 border p-6 rounded-xl shadow-md bg-white flex flex-col justify-center items-center"
              >
                <h4 class="text-2xl font-bold mb-4">Premium Plan</h4>
                <p class="text-gray-500 text-lg mb-6">$49 / mo</p>
                <ul class="text-gray-600 space-y-3 mb-6">
                  <li>Unlimited Projects</li>
                  <li>500K API Access</li>
                  <li>1GB Storage</li>
                  <li>Daily Reports</li>
                  <li>Priority Support</li>
                </ul>
                <button class="bg-blue-500 text-white px-6 py-2 rounded-full">
                  Choose Plan
                </button>
              </div>
            </div>

            <div v-else key="yearly" class="flex justify-center gap-6">
              <div
                class="w-80 h-96 border p-6 rounded-xl shadow-md bg-white flex flex-col justify-center items-center"
              >
                <h4 class="text-2xl font-bold mb-4">Basic Plan</h4>
                <p class="text-gray-500 text-lg mb-6">$199 / yr</p>
                <ul class="text-gray-600 space-y-3 mb-6">
                  <li>5 Projects</li>
                  <li>100K API Access</li>
                  <li>200MB Storage</li>
                  <li>Weekly Reports</li>
                  <li>24/7 Support</li>
                </ul>
                <button class="bg-blue-500 text-white px-6 py-2 rounded-full">
                  Choose Plan
                </button>
              </div>

              <div
                class="w-80 h-96 border p-6 rounded-xl shadow-md bg-white flex flex-col justify-center items-center"
              >
                <h4 class="text-2xl font-bold mb-4">Premium Plan</h4>
                <p class="text-gray-500 text-lg mb-6">$499 / yr</p>
                <ul class="text-gray-600 space-y-3 mb-6">
                  <li>Unlimited Projects</li>
                  <li>500K API Access</li>
                  <li>1GB Storage</li>
                  <li>Daily Reports</li>
                  <li>Priority Support</li>
                </ul>
                <button class="bg-blue-500 text-white px-6 py-2 rounded-full">
                  Choose Plan
                </button>
              </div>
            </div>
          </transition>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.2s;
}
.fade-enter,
.fade-leave-to {
  opacity: 0;
}
</style>
<script setup>
import { ref } from "vue";

const isMonthly = ref(true);

const togglePricing = () => {
  isMonthly.value = !isMonthly.value;
};
</script>
