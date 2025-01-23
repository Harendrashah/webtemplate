<template>
  <div>
    <!-- upper part with readMore button -->
    <DemoUpper />

    <!-- second part -->
    <div class="flex flex-col md:h-[90vh] mt-11 items-center xl:mt-[140px]">
      <span class="text-gray-500">WHAT WE DO?</span>
      <h1
        class="text-[40px] text-center text-[#353F53] mb-9 font-bold leading-snug sm:text-[30px] md:mt-[15px] md:text-[33px] lg:text-[40px] md:max-w-[673px]"
      >
        The service we offer is specifically designed to meet your needs.
      </h1>

      <!-- Grid with  servide cardcards -->
      <div class="w-full max-w-[1300px] mx-auto px-4">
        <div class="pb-10">
          <div class="grid grid-cols-1 md:grid-cols-3 gap-5">
            <DemoService
              v-for="(item, index) in description"
              :key="index"
              :card="item"
            />
          </div>
        </div>
      </div>
    </div>

    <!-- Third part -->

    <div class="flex flex-col md:h-[100vh] mt-11 md:flex-row bg-[#F6F6F8]">
      <!-- Image Section -->
      <div class="h-full w-full md:w-1/2">
        <img
          src="@/assets/icons/bgimg.svg"
          alt="bg39"
          class="object-cover h-full"
        />
      </div>

      <!-- Content Section -->
      <div class="flex flex-col items-start justify-center p-6 md:ml-10">
        <!-- Heading Section -->

        <!-- Service Cards -->
        <div class="space-y-4 mt-28 md:mt-0">
          <div class="mb-6">
            <span class="text-[#AEB0BC] mb-3 text-[18px] block"
              >HOW IT WORKS?</span
            >
            <h1
              class="text-[#353F53] font-bold text-[30px] leading-snug max-w-[400px] sm:text-[20px] md:text-[25px] lg:text-[30px]"
            >
              Here are the 3 working steps to success.
            </h1>
          </div>

          <DemoService
            v-for="(item, index) in whatWorks"
            :key="index"
            :card="item"
          />
        </div>
      </div>
    </div>

    <!-- fourth -->
    <div
      class="flex flex-col items-center mt-11 md:h-[100vh] justify-center space-y-8"
    >
      <!-- Heading Section -->
      <div class="lg:max-w-[450px] text-center mb-8">
        <span class="text-gray-500 font-bold uppercase tracking-wide"
          >Case Study</span
        >
        <h1 class="text-[2rem] text-[#353F53] font-bold mt-2 leading-snug">
          Our awesome project with great ideas and design
        </h1>
      </div>

      <!-- Cards Section -->
      <div class="flex flex-wrap justify-center gap-6 mt-8">
        <DemoCaseCard
          v-for="(item, index) in cases"
          :key="index"
          :card="item"
        />
      </div>
    </div>

    <!-- fifth -->
    <div
      class="flex flex-col mt-11 md:flex-row h-[100vh] bg-gray-300 items-center justify-center"
    >
      <!-- Text Section -->
      <div
        class="flex flex-col items-center justify-center w-full md:w-1/2 p-6 text-center md:text-left"
      >
        <div class="max-w-[533px]">
          <span class="text-lg font-semibold text-gray-700">Our Solution</span>
          <h2 class="mt-4 text-[40px] font-normal text-gray-900 leading-tight">
            Just sit & relax while we take care of your business needs.
          </h2>
          <p class="mt-4 text-[16px] text-gray-600">
            Cum sociis natoque penatibus et magnis dis parturient montes,
            nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in,
            egestas eget quam. Praesent commodo cursus. Maecenas sed diam eget
            risus varius blandit sit amet non magna. Praesent commodo cursus
            magna.
          </p>
          <div class="flex mt-5 gap-5">
            <div class="flex flex-col">
              <span class="text-[44px]">97.7%</span>
              <span class="text-[19px]">Customer Satisfaction</span>
              <img
                src="../assets/icons/rating.svg"
                class="md:w-[90px] w-[90px] mt-[8px]"
              />
            </div>
            <div class="flex flex-col">
              <span class="text-[44px]">4X</span>
              <span class="text-[19px]">New Visitor</span>
              <img
                src="../assets/icons/rating.svg"
                class="md:w-[90px] w-[90px] mt-[8px]"
              />
            </div>
          </div>
        </div>
      </div>

      <!-- Image Section -->
      <div class="flex items-center justify-center w-full md:w-1/2 h-full">
        <img
          src="@/assets/images/bg39.jpg"
          alt="bg39"
          class="w-auto max-h-[80%] object-contain rounded-md shadow-lg"
        />
      </div>
    </div>

    <!-- sixth -->
    <div
      class="flex flex-col md:h-[100vh] w-full md:flex-row mt-20 items-center md:items-start bg-gray-100 p-6 space-y-6 md:space-y-0 md:space-x-6"
    >
      <!-- Image Section -->
      <div class="flex flex-col ml-0 md:ml-10">
        <!-- First Row of Images -->
        <div class="flex flex-col md:flex-row mb-[25px]">
          <img
            src="@/assets/images/g14.jpg"
            class="rounded-md md:w-[292px] md:h-[259px] mr-[25px]"
            alt="Image 14"
          />
          <img
            src="@/assets/images/g15.jpg"
            class="rounded-md md:w-[292px] md:h-[234px] mt-6"
            alt="Image 15"
          />
        </div>
        <!-- Second Row of Image -->
        <img
          src="@/assets/images/g16.jpg"
          class="mt-4 rounded-md w-[560px] h-[285px]"
          alt="Image 16"
        />
      </div>

      <!-- Text Section -->
      <div class="flex flex-col max-w-lg md:ml-8 justify-center">
        <span class="text-gray-500 uppercase tracking-wide text-[15px]"
          >Who are we?</span
        >
        <h2 class="text-[40px] md:text-3xl text-gray-800 mt-2">
          Company that believes in the power of creative strategy.
        </h2>
        <p class="text-gray-600 text-[18px] md:text-base mt-4 leading-relaxed">
          Cum sociis natoque penatibus et magnis dis parturient montes, nascetur
          ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget
          quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur
          et. Cum sociis natoque penatibus et magnis dis parturient montes,
          nascetur ridiculus mus. Aenean lacinia bibendum nulla sed.
        </p>
        <div class="grid grid-cols-2 gap-5 mt-[20px]">
          <div class="flex mt-2">
            <img src="../assets/icons/check.svg" class="mr-2 -mt-3" />
            <span>Aenean eu leo quam ornare curabitur blandit tempus.</span>
          </div>
          <div class="flex mt-2">
            <img src="../assets/icons/check.svg" class="mr-2 -mt-3" />
            <span>Aenean eu leo quam ornare curabitur blandit tempus.</span>
          </div>
          <div class="flex mt-2">
            <img src="../assets/icons/check.svg" class="mr-2 -mt-3" />
            <span>Aenean eu leo quam ornare curabitur blandit tempus.</span>
          </div>
          <div class="flex mt-2">
            <img src="../assets/icons/check.svg" class="mr-2 -mt-3" />
            <span>Aenean eu leo quam ornare curabitur blandit tempus.</span>
          </div>
        </div>
      </div>
    </div>

    <div class="grid grid-cols-1 ml-5 md:grid-cols-3 gap-4 mt-8">
      <DemoService
        v-for="(item, index) in whatWorks"
        :key="index"
        :card="item"
      />
    </div>
    <!-- Service pack plan of business -->

    <div class="flex md:mt-24 md:ml-[150px]">
      <div
        class="relative md:w-[960px] md:h-[494px] bg-gray-100 p-8 rounded-md"
      >
        <!-- Text Content -->
        <div class="max-w-[435px] items-center justify-center">
          <img
            src="../assets/icons/rating.svg"
            class="md:ml-[140px] mb-5 ml-5 items-center"
          />
          <span class="text-gray-800 md:text-[20px]">
            “Donec id elit non mi porta gravida at eget metus. Vivamus mollis
            est non commodo luctus, nisi erat porttitor ligula, eget lacinia
            odio sem nec elit. Duis mollis porta est non commodo luctus.”
          </span>
        </div>

        <!-- Image -->
        <img
          src="../assets/images/tei1.jpg"
          class="md:absolute md:right-[-290px] mt-24 transform -translate-y-1/2 rounded-lg"
          alt="Overlapping Image"
        />
      </div>
    </div>

    <!-- <div class="flex flex-col w-full md:flex-row items-center">
    <DemoPlans/>
    <DemoPlans/>
    <DemoPlans/>
    <DemoPlans/>
    
  </div> -->

    <div class="p-5">
      <DemoHappyclinet />
      <DemoOurclient />
    </div>

    <!-- <section class="wrapper !bg-[#ffffff] angled upper-end lower-end relative border-0 
    before:top-[-4rem] before:border-l-transparent before:border-r-[100vw] 
    before:border-t-[4rem] before:border-[#0000FF] before:content-[''] before:block 
    before:absolute before:z-0 before:!border-y-transparent before:border-0 
    before:border-solid before:right-0 
    after:bottom-[-4rem] after:border-l-transparent after:border-r-[100vw] 
    after:border-b-[4rem] after:border-[#0000FF] after:content-[''] after:block 
    after:absolute after:z-0 after:!border-y-transparent after:border-0 
    after:border-solid after:right-0">
  </section> -->
  </div>
</template>
<script setup>
import image1 from "@/assets/icons/24Support.svg";
import image2 from "@/assets/icons/secondservice.svg";
import image3 from "@/assets/icons/colud.svg";
import case1 from "@/assets/images/b4.jpg";
import case2 from "@/assets/images/b5.jpg";
import case3 from "@/assets/images/b6.jpg";

const description = [
  {
    title: "12 hr Support",
    description:
      "odiosem aget elit nullam quis risus eget duis mollis gravida commodo id lucerat porttitor ligula, eget lacinia ",
    image: image1,
  },

  {
    title: "Secure Payment",
    description:
      "odiosem aget elit nullam quis risus eget duis mollis gravida commodo id lucerat porttitor ligula, eget lacinia ",
    image: image2,
  },

  {
    title: "Daily Updates",
    description:
      "Duis mollis gravida commodo id lucerat porttitor ligula, eget lacinia odiosem aget elit nullam quis risus eget.",
    image: image3,
  },

  {
    title: "Market research",
    description:
      "odiosem aget elit nullam quis risus eget duis mollis gravida commodo id lucerat porttitor ligula, eget lacinia .",
    image: image2,
  },

  {
    title: "Social Engagement",
    description:
      "Duis mollis gravida commodo id lucerat porttitor ligula, eget lacinia odiosem aget elit nullam quis risus eget.",
    image: image1,
  },

  {
    title: "Content Marketing",
    description:
      "Commodo id lucerat duis mollis gravida commodo id lucerat porttitor ligula, eget lacinia odiosem aget elit nullam quis risus eget.",
    image: image3,
  },
];

const cases = [
  {
    task: "Coding",
    date: "12/2/4",
    title: "The status project",
    image: case1,
  },
  {
    task: "Workspace",
    date: "12/2/4",
    title: "The Next Project",
    image: case2,
  },
  {
    task: "Design",
    date: "12/2/4",
    title: "lorem chorem dhorem",
    image: case3,
  },
];

const whatWorks = [
  {
    title: "24/7 Support",
    description:
      "Nulla vitae elit libero pharetra augue dapibu Praesent commodo cursus",
    image: image1,
  },

  {
    title: "Secure payment",
    description:
      "Nulla vitae elit libero pharetra augue dapibu Praesent commodo cursus",
    image: image3,
  },

  {
    title: "Daily updates",
    description:
      "Nulla vitae elit libero pharetra augue dapibu Praesent commodo cursus",
    image: image2,
  },
];
</script>
<style>
.clip-triangle {
  clip-path: polygon(0 100%, 50% 0, 100% 100%);
}
</style>
