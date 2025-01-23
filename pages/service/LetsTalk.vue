<template>
  <div class="flex flex-col md:flex-row items-start gap-8 p-6 mt-7">
    <div class="md:ml-[80px] mt-9">
      <!-- <div
        class="shape bg-dot primary rellax !w-[8rem] !h-[8rem] bg-[radial-gradient(#3f78e0_2px,transparent_2.5px)] absolute z-[1] opacity-50"
        data-rellax-speed="1"
        style="
          top: 0px;
          left: -1.4rem;
          z-index: 0;
          transform: translate3d(0px, -6px, 0px);
        "
      ></div> -->

      <img
        src="https://sandbox-tailwind-template.netlify.app/assets/img/photos/g5.jpg"
        alt="Image 1"
        class="w-[600px] h-[300px] rounded-md shadow-md"
      />
    </div>

    <div class="flex flex-col items-center gap-4">
      <div
        class="bg-[#EDF3FD] w-[300px] flex-col h-[200px] rounded-md flex items-center justify-center"
      >
        <span class="text-2xl font-bold">5000+</span>
        <span class="text-md">Satisfied Customers</span>
      </div>

      <img
        src="https://sandbox-tailwind-template.netlify.app/assets/img/photos/g6.jpg"
        alt="Image 2"
        class="w-full max-w-[300px] rounded-md shadow-md"
      />
    </div>

    <div class="flex flex-col gap-8">
      <h1 class="text-[40px] md:w-[550px] font-bold">Let’s Talk</h1>

      <div class="flex flex-col gap-6">
        <div class="flex flex-col items-start">
          <p
            class="lead !text-[1.2rem] !leading-[1.6] font-medium text-gray-600"
          >
            Let's make something great together. We are
            <span
              class="relative z-[2] whitespace-nowrap after:content-[''] after:block after:absolute after:w-[102.5%] after:h-[30%] after:left-[-1.5%] after:z-[-1] after:transition-all after:duration-[0.2s] after:ease-in-out after:mt-0 after:rounded-[5rem] after:bottom-[9%] motion-reduce:after:transition-none after:bg-[rgba(63,120,224,.12)]"
              >trusted by</span
            >
            over 5000+ clients. Join them by using our services and grow your
            business.
          </p>
          <p class="text-gray-500">
            Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis
            vestibulum. Maecenas faucibus mollis interdum. Fusce dapibus, tellus
            ac cursus commodo, tortor mauris condimentum nibh, ut fermentum
            massa justo sit amet risus.
          </p>
          <a
            href="#"
            class="w-[100px] h-[40px] text-center mt-4 flex items-center justify-center font-bold text-white text-[20px] !bg-[#3f78e0] border-[#3f78e0] hover:text-white hover:bg-[#3f78e0] hover:border-[#3f78e0] focus:shadow-[rgba(92,140,229,1)] active:text-white active:bg-[#3f78e0] active:border-[#3f78e0] disabled:text-white disabled:bg-[#3f78e0] disabled:border-[#3f78e0] !rounded-[50rem] hover:translate-y-[-0.15rem] hover:shadow-[0_0.25rem_0.75rem_rgba(30,34,40,0.15)]"
            >Join Us</a
          >
        </div>
      </div>
    </div>
  </div>
</template>
