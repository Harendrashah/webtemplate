<template>
  <div class="w-full  flex flex-col top-0 h-full">
    <img
      src="../../../assets/bg/bluebg.svg"
      alt="background"
      class="absolute object-cover inset-0 w-full mt-10 z-0"
    />
    <div
      class="relative flex flex-col bg-none items-center justify-center bg-cover bg-center rounded-b-[400px] py-10"
    >
      <span
        class="relative z-10 block font-bold text-lg text-[15px] text-gray-300"
      >
        Join our Team
      </span>
      <span
        class="relative z-10 block mt-2 text-[32px] md:text-[48px] md:w-[720px] font-extrabold text-center text-gray-500"
      >
        Join our team to help shape the future of development.
      </span>
      <button
        class="relative z-10 bg-[#3F78E0] h-[59px] px-[30px] rounded-full flex items-center justify-center text-[20px] text-white font-bold mt-5"
      >
        Explore Position
      </button>
    </div>

    <div
      class="relative  -mt-5 z-20 md:pl-[50px] md:pr-[50px] flex flex-wrap justify-center gap-5"
    >
      <CareerCardTop />
      <CareerCardTop />
      <CareerCardTop />
      <CareerCardTop />
    </div>
  </div>
</template>
