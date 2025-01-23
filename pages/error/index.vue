<template>
  <div>
    <div class="bg-[#ffffff] h-[100% ] w-[100%]">
      <div class="flex justify-center items-center flex-col gap-4">
        <img
          src="https://sandbox-tailwind-template.netlify.app/assets/img/illustrations/404.png"
          alt=""
          class="h-[90%] w-[50%] mt-[6rem]"
        />
        <div class="font-bold font-sans text-[40px] text-[#304056]">
          Oops! Page Not Found.
        </div>
        <div class="font-sans text-[30px] font-medium w-[881px] text-[#656b74]">
          The page you are looking for is not available or has been moved. Try a
          different page or go to homepage with the button below.
        </div>
        <NuxtLink to="/">
          <button
            class="bg-[#3f78e1] w-[141%] h-[85px] outline-none rounded-full cursor-pointer font-sans font-semibold text-[30px] text-white mt-7"
          >
            Go To HomePage
          </button>
        </NuxtLink>
        <!-- <DemoOurclient /> -->
      </div>
    </div>
  </div>
</template>
