<template>
  <div class="flex flex-col md:mb-[200px] md:flex-row md:items-center md:mt-32 md:px-32">
    <!-- Image Section -->
    <div class="flex flex-col md:w-1/2 gap-4 md:pr-8">
      <!-- Main Image -->
      <img
        src="https://sandbox-tailwind-template.netlify.app/assets/img/photos/g8.jpg"
        alt="Main Image"
        class="w-full rounded-lg object-cover"
      />

      <div class="flex gap-4">
        <img
          src="https://sandbox-tailwind-template.netlify.app/assets/img/photos/g9.jpg"
          alt="Sub Image 1"
          class="w-1/2 rounded-lg object-cover"
        />
        <img
          src="https://sandbox-tailwind-template.netlify.app/assets/img/photos/g10.jpg"
          alt="Sub Image 2"
          class="w-1/2 rounded-lg object-cover"
        />
      </div>
    </div>

    <!-- Context Section -->
    <div
      class="flex flex-col md:w-1/2 md:pl-8 md:-mt-20 text-center md:text-left"
    >
      <h2 class="text-2xl md:text-4xl font-bold mb-4 leading-snug">
        We bring solutions to make life easier for our customers.
      </h2>
      <p class="text-sm md:text-base text-gray-600 leading-relaxed">
        Etiam porta sem malesuada magna mollis euismod. Cum sociis natoque
        penatibus et magnis dis parturient montes, nascetur ridiculus mus. Nulla
        vitae elit libero, a pharetra augue. Etiam porta sem malesuada magna
        mollis euismod. Cras justo odio, dapibus ac facilisis in, egestas eget
        quam. Maecenas sed.
      </p>
      <div class="flex-col flex md:flex-row mt-5 ">
        <div class="flex items-center gap-4">
          <!-- Icon Image -->
          <img
            src="../../../assets/icons/carrier.svg"
            alt="image"
            class="w-8 h-8 -mt-10 object-cover rounded-lg"
          />

          <!-- Text Section of card -->
          <div class="flex flex-col -ml-">
            <span class="text-xl font-semibold text-gray-800">Our Mission</span>
            <span class="text-sm text-gray-600 mt-1"
              >Curabitur blandit lacus porttitor ridiculus mus</span
            >
          </div>
        </div>

        <div class="flex items-center gap-4 md: ml-5">
          <!-- Icon Image -->
          <img
            src="../../../assets/icons/carrier.svg"
            alt="image"
            class="w-8 h-8 -mt-10 object-cover rounded-lg"
          />

          <!-- Text Section -->
          <div class="flex flex-col">
            <span class="text-xl font-semibold text-gray-800">Our Mission</span>
            <span class="text-sm text-gray-600 mt-1"
              >Curabitur blandit lacus porttitor ridiculus mus</span
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
