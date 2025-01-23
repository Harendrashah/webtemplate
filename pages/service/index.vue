<template>
  <div class="mb-5 overflow-hidden bg-none  w-full h-full">
    <div class="w-full h-[400px] bg-[#EDF2FC]">
      <div class="relative z-10 pt-10 pb-36 px-7">
        <div class="flex flex-col justify-center items-center">
          <h1
            class="text-[calc(1.365rem_+_1.38vw)] mt-9 font-bold leading-[1.2] xl:text-[2.4rem] !mb-3"
          >
            Our Services
          </h1>
          <p
            class="lead leading-[1.65] text-[0.9rem] w-[550px] text-center font-[16px]  lg:!px-7 xl:!px-7 xxl:!px-6 text-gray-600"
          >
            We are a creative company that focuses on establishing
            <span
              class="relative z-[2] whitespace-nowrap after:content-[''] after:block after:absolute after:w-[102.5%] after:h-[30%] after:left-[-1.5%] after:z-[-1] after:transition-all after:duration-[0.2s] after:ease-in-out after:mt-0 after:rounded-[5rem] after:bottom-[9%] motion-reduce:after:transition-none after:bg-[rgba(63,120,224,.12)]"
              >long-term relationships</span
            >
            with customers.
          </p>
        </div>
      </div>
    </div>
    <div
      class="bottom-0 w-full h-[60px] -rotate-2 origin-bottom-left bg-white"
    ></div>

    <div>
        <div class="relative px-[100px]">
      <div class="mt-[-150px] ml-[50px]">
        <img
          src="https://sandbox-tailwind-template.netlify.app/assets/img/photos/about5.jpg"
          alt="About Image"
          class="w-[100%] h-[550px] object-cover rounded-lg"
        />
      </div>
      <div class="w-[90%] ml-[87px]">
        <div
          class="card image-wrapper bg-full bg-image rounded-xl bg-overlay bg-overlay-400 text-white mt-[-1.25rem] xl:!mt-0 lg:!mt-0 xl:-translate-y-2/4 lg:-translate-y-2/4 bg-cover [background-size:100%] bg-[center_center] bg-no-repeat !bg-scroll !relative z-0 before:content-[''] before:block before:absolute before:z-[1] before:w-full before:h-full before:left-0 before:top-0"
          data-image-src="./assets/img/photos/bg3.jpg"
          style="
            background-image: url('https://sandbox-tailwind-template.netlify.app/assets/img/photos/bg3.jpg');
          "
        >
          <div class="card-body p-[2.25rem] xl:!p-[2.5rem]">
            <div
              class="flex flex-wrap mx-[-15px] items-center counter-wrapper mt-[-20px] !text-center"
            >
              <div
                class="w-6/12 xl:w-3/12 lg:w-3/12 flex-[0_0_auto] px-[15px] max-w-full mt-[20px]"
              >
                <h3
                  class="counter counter-lg text-white xl:text-[2.2rem] text-[calc(1.345rem_+_1.14vw)] font-bold font-sans tracking-[normal] !leading-none mb-2"
                  style="visibility: visible"
                >
                  7518
                </h3>
                <p class="text-[1rem] font-medium !mb-0 text-white">
                  Completed Projects
                </p>
              </div>
              <div
                class="w-6/12 xl:w-3/12 lg:w-3/12 flex-[0_0_auto] px-[15px] font-bold font-sans max-w-full mt-[20px]"
              >
                <h3
                  class="counter counter-lg text-white xl:text-[2.2rem] font-bold font-sans text-[calc(1.345rem_+_1.14vw)] tracking-[normal] !leading-none mb-2"
                  style="visibility: visible"
                >
                  3472
                </h3>
                <p class="text-[1rem] font-medium !mb-0 text-white">
                  Satisfied Customers
                </p>
              </div>
              <div
                class="w-6/12 xl:w-3/12 lg:w-3/12 flex-[0_0_auto] px-[15px] max-w-full mt-[20px]"
              >
                <h3
                  class="counter counter-lg text-white xl:text-[2.2rem] font-bold font-sans text-[calc(1.345rem_+_1.14vw)] tracking-[normal] !leading-none mb-2"
                  style="visibility: visible"
                >
                  2184
                </h3>
                <p class="text-[1rem] font-medium !mb-0 text-white">
                  Expert Employees
                </p>
              </div>
              <div
                class="w-6/12 xl:w-3/12 lg:w-3/12 flex-[0_0_auto] px-[15px] max-w-full mt-[20px]"
              >
                <h3
                  class="counter counter-lg text-white xl:text-[2.2rem] font-bold font-sans text-[calc(1.345rem_+_1.14vw)] tracking-[normal] !leading-none mb-2"
                  style="visibility: visible"
                >
                  4523
                </h3>
                <p class="text-[1rem] font-medium !mb-0 text-white">
                  Awards Won
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <WeDo />
    <StressFree />
    
      <!-- Parallax Section -->
      <div class="parallax-section  ">
        <div class=""></div>
        <h1 class="text-center absolute text-white pt-32 text-4xl font-bold w-[650px]">Find out everything you need to know about creating a business process model.</h1>
      </div>
      <section class="wrapper !bg-[#ffffff] angled  mb-8 upper-end lower-end relative border-0 
    before:top-[-4rem] before:border-l-transparent before:border-r-[100vw] 
    before:border-t-[4rem] before:border-[#ffffff] before:content-[''] before:block 
    before:absolute before:z-0 before:!border-y-transparent before:border-0 
    before:border-solid before:right-0 
    after:bottom-[-4rem] after:border-l-transparent after:border-r-[100vw] 
    after:border-b-[4rem] after:border-[#ffffff] after:content-[''] after:block 
    after:absolute after:z-0 after:!border-y-transparent after:border-0 
    after:border-solid after:right-0"></section>
  
  
   
      <OurPricing />
      <LetsTalk />
      
    </div>
   
  
    <!-- <VideoFixing /> -->
    
  </div>
</template>
<script setup>
import StressFree from "./StressFree.vue";
import WeDo from "./WeDo.vue";
import LetsTalk from "./LetsTalk.vue";
import OurPricing from "./OurPricing.vue";

</script>

<style scoped>
/* Parallax Section */
.parallax-section {
  height: 60vh; 
  margin-top: 100px;
  background-image: url("https://sandbox-tailwind-template.netlify.app/assets/img/photos/bg1.jpg");
  background-attachment: fixed; 
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgba(0, 0, 0, 1); 
  z-index: 1; 
}


</style>