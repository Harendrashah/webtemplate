<template>
  <div>
    <footer>
      <div class="bg-[#f6f7f9] p-8 md:p-16 lg:p-28 w-full">
        <div
          class="flex flex-col lg:flex-row justify-between items-center text-center lg:text-left"
        >
          <div
            class="font-sans font-bold text-[25px] lg:text-[35px] lg:w-[550px] h-auto mb-4 lg:mb-0"
          >
            Join our community by using our services and grow your business.
          </div>
          <div
            class="bg-black w-full lg:w-[220px] flex justify-center items-center font-sans font-semibold text-[20px] lg:text-[25px] h-[60px] lg:h-[80px] text-gray-200 rounded-xl border cursor-pointer"
          >
            Try It For Free
          </div>
        </div>

        <div class="border rounded-2xl mt-7 mb-12"></div>

        <div
          class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12 md:gap-16"
        >
          <div class="flex flex-col items-center lg:items-start">
            <div class="mb-3">
              <img
                src="https://yajtechnologies.com/assets/newtheme/img/logo.png"
                alt="Logo"
                class="w-[160px] object-cover"
              />
            </div>
            <!-- <img
              src="https://sandbox-tailwind-template.netlify.app/assets/img/logo-dark.png"
              alt="Logo"
              class="w-[150px] lg:w-[177px] mb-4"
            /> -->
            <div class="text-gray-500 text-[16px] lg:text-[18px] mb-4">
              <div>© 2024 Sandbox.</div>
              <div>All rights reserved.</div>
            </div>

            <div class="flex gap-3 md:gap-4">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="25"
                height="25"
                fill="currentColor"
                class="hover:text-[#343f52] cursor-pointer"
                viewBox="0 0 512 512"
              >
                <path
                  d="M459.4 151.7c.3 4.5 .3 9.1 .3 13.6 0 138.7-105.6 298.6-298.6 298.6-59.5 0-114.7-17.2-161.1-47.1 8.4 1 16.6 1.3 25.3 1.3 49.1 0 94.2-16.6 130.3-44.8-46.1-1-84.8-31.2-98.1-72.8 6.5 1 13 1.6 19.8 1.6 9.4 0 18.8-1.3 27.6-3.6-48.1-9.7-84.1-52-84.1-103v-1.3c14 7.8 30.2 12.7 47.4 13.3-28.3-18.8-46.8-51-46.8-87.4 0-19.5 5.2-37.4 14.3-53 51.7 63.7 129.3 105.3 216.4 109.8-1.6-7.8-2.6-15.9-2.6-24 0-57.8 46.8-104.9 104.9-104.9 30.2 0 57.5 12.7 76.7 33.1 23.7-4.5 46.5-13.3 66.6-25.3-7.8 24.4-24.4 44.8-46.1 57.8 21.1-2.3 41.6-8.1 60.4-16.2-14.3 20.8-32.2 39.3-52.6 54.3z"
                />
              </svg>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="25"
                height="25"
                fill="currentColor"
                class="hover:text-[#343f52] cursor-pointer"
                viewBox="0 0 512 512"
              >
                <path
                  d="M512 256C512 114.6 397.4 0 256 0S0 114.6 0 256C0 376 82.7 476.8 194.2 504.5V334.2H141.4V256h52.8V222.3c0-87.1 39.4-127.5 125-127.5c16.2 0 44.2 3.2 55.7 6.4V172c-6-.6-16.5-1-29.6-1c-42 0-58.2 15.9-58.2 57.2V256h83.6l-14.4 78.2H287V510.1C413.8 494.8 512 386.9 512 256h0z"
                />
              </svg>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="25"
                height="25"
                fill="currentColor"
                class="hover:text-[#343f52] cursor-pointer"
                viewBox="0 0 448 512"
              >
                <path
                  d="M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.1 0-74.7-33.5-74.7-74.7s33.5-74.7 74.7-74.7 74.7 33.5 74.7 74.7-33.6 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.8-26.8 26.8-14.9 0-26.8-12-26.8-26.8s12-26.8 26.8-26.8 26.8 12 26.8 26.8zm76.1 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM398.8 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z"
                />
              </svg>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="25"
                height="25"
                fill="currentColor"
                class="hover:text-[#343f52] cursor-pointer"
                viewBox="0 0 512 512"
              >
                <path
                  d="M256 8C119.3 8 8 119.3 8 256s111.3 248 248 248 248-111.3 248-248S392.7 8 256 8zm164 114.4c29.5 36 47.4 82 47.8 132-7-1.5-77-15.7-147.5-6.8-5.8-14-11.2-26.4-18.6-41.6 78.3-32 113.8-77.5 118.3-83.5zM396.4 97.9c-3.8 5.4-35.7 48.3-111 76.5-34.7-63.8-73.2-116.2-79-124 67.2-16.2 138 1.3 190.1 47.5zm-230.5-33.3c5.6 7.7 43.4 60.1 78.5 122.5-99.1 26.3-186.4 25.9-195.8 25.8C62.4 147.2 106.7 92.6 165.9 64.6zM44.2 256.3c0-2.2 0-4.3 .1-6.5 9.3 .2 111.9 1.5 217.7-30.1 6.1 11.9 11.9 23.9 17.2 35.9-76.6 21.6-146.2 83.5-180.5 142.3C64.8 360.4 44.2 310.7 44.2 256.3zm81.8 167.1c22.1-45.2 82.2-103.6 167.6-132.8 29.7 77.3 42 142.1 45.2 160.6-68.1 29-150 21.1-212.8-27.9zm248.4 8.5c-2.2-12.9-13.4-74.9-41.2-151 66.4-10.6 124.7 6.8 131.9 9.1-9.4 58.9-43.3 109.8-90.8 142z"
                />
              </svg>
            </div>
          </div>

          <div class="text-center lg:text-left">
            <h2
              class="text-gray-600 font-sans font-semibold text-[20px] lg:text-[30px] mb-4"
            >
              Get in Touch
            </h2>
            <p class="text-gray-500 text-[16px] lg:text-[18px]">
              Moonshine St. 14/05 Light City, London, United Kingdom
            </p>
            <p class="text-gray-500 text-[16px] lg:text-[18px]">
              info@email.com
            </p>
            <p class="text-gray-500 text-[16px] lg:text-[18px]">9845337129</p>
          </div>

          <div>
            <h2
              class="text-gray-600 font-sans font-semibold text-[20px] lg:text-[30px] mb-4"
            >
              Learn More
            </h2>
            <ul class="space-y-2">
              <li>
                <a
                  class="text-gray-500 hover:text-[#343f52] text-[16px] lg:text-[18px]"
                  href="#"
                  >About Us</a
                >
              </li>
              <li>
                <a
                  class="text-gray-500 hover:text-[#343f52] text-[16px] lg:text-[18px]"
                  href="#"
                  >Our Story</a
                >
              </li>
              <li>
                <a
                  class="text-gray-500 hover:text-[#343f52] text-[16px] lg:text-[18px]"
                  href="#"
                  >Projects</a
                >
              </li>
              <NuxtLink to="/terms/TermsCondition">
                <li>
                  <a
                    class="text-gray-500 hover:text-[#343f52] text-[16px] lg:text-[18px]"
                    href="#"
                    >Terms of Use</a
                  >
                </li>
              </NuxtLink>

              <li>
                <a
                  class="text-gray-500 hover:text-[#343f52] text-[16px] lg:text-[18px]"
                  href="#"
                  >Privacy Policy</a
                >
              </li>
            </ul>
          </div>

          <div class="text-center lg:text-left">
            <h2
              class="text-gray-600 font-sans font-semibold text-[20px] lg:text-[30px] mb-4"
            >
              Our Newsletter
            </h2>
            <p class="text-gray-500 text-[16px] lg:text-[18px] mb-4">
              Subscribe to our newsletter to get our news & deals delivered to
              you.
            </p>
            <div class="flex flex-col lg:flex-row">
              <input
                type="text"
                placeholder="Email Address"
                class="h-[40px] lg:h-[50px] w-full lg:w-[250px] rounded-xl lg:rounded-l-xl p-3"
              />
              <button
                class="w-full lg:w-[100px] h-[40px] lg:h-[50px] bg-[#3f78e1] text-white text-[18px] lg:text-[22px] rounded-xl lg:rounded-r-xl"
              >
                Join
              </button>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>
