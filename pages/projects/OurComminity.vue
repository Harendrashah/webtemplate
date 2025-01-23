<script setup lang="ts">
import SalesFinance from "./SalesFinance.vue";
</script>

<template>
  <div>
    <section class="wrapper bg-white">
      <div class="container pt-20 xl:pt-28 pb-16 xl:pb-20">
        <div class="flex flex-wrap items-start">
          <div class="xl:w-4/12 w-full px-4">
            <h2 class="text-2xl xl:text-4xl font-bold leading-snug mb-4">
              Our Community
            </h2>
            <p class="text-lg text-gray-600 leading-relaxed mb-6">
              Customer satisfaction is our major goal. See what our clients are
              saying about our services.
            </p>
            <a
              href="#"
              class="inline-block px-6 py-3 bg-blue-600 text-white font-medium rounded-full shadow-lg transition hover:bg-blue-500"
            >
              All Testimonials
            </a>
          </div>

          <div class="w-full px-4 mt-8 xl:mt-0">
            <div class="relative">
              <div
                class="absolute top-0 right-[-1rem] bg-orange-100 rounded-full w-24 h-24"
              ></div>
              <div
                class="absolute bottom-[-1rem] left-[-1.5rem] bg-red-100 rounded-full w-24 h-24 opacity-50"
              ></div>

              <div class="swiper-container relative">
                <div class="swiper-wrapper">
                  <div class="flex gap-8">
                    <!-- Increased gap here -->
                    <div class="swiper-slide flex w-1/2">
                      <div class="bg-white shadow-lg rounded-lg p-6">
                        <blockquote class="text-gray-800 text-lg italic mb-4">
                          "Maecenas faucibus mollis interdum. Duis mollis, est
                          non commodo luctus, nisi erat porttitor ligula, eget
                          lacinia odio sem nec elit. Praesent commodo cursus
                          magna, vel scelerisque."
                        </blockquote>
                        <div class="flex items-center">
                          <img
                            class="w-16 h-16 rounded-full"
                            src="https://sandbox-tailwind-template.netlify.app/assets/img/avatars/te1.jpg"
                            alt="User"
                          />
                          <div class="ml-4">
                            <h5 class="text-base font-semibold">
                              Jackie Sanders
                            </h5>
                            <p class="text-sm text-gray-500">
                              Investment Planner
                            </p>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="swiper-slide flex w-1/2">
                      <div class="bg-white shadow-lg rounded-lg p-6">
                        <blockquote class="text-gray-800 text-lg italic mb-4">
                          "Sed posuere consectetur est at lobortis. Nulla vitae
                          elit libero, a pharetra augue. Lorem ipsum dolor sit
                          amet, consectetur adipiscing elit."
                        </blockquote>
                        <div class="flex items-center">
                          <img
                            class="w-16 h-16 rounded-full"
                            src="https://sandbox-tailwind-template.netlify.app/assets/img/avatars/te2.jpg"
                            alt="User"
                          />
                          <div class="ml-4">
                            <h5 class="text-base font-semibold">John Doe</h5>
                            <p class="text-sm text-gray-500">Product Manager</p>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>

                  <div class="flex gap-8 mt-5">
                    <!-- Increased gap here -->
                    <div class="swiper-slide flex w-1/2">
                      <div class="bg-white shadow-lg rounded-lg p-6">
                        <blockquote class="text-gray-800 text-lg italic mb-4">
                          "Phasellus viverra nulla ut metus varius laoreet. Sed
                          posuere consectetur est at lobortis. Lorem ipsum dolor
                          sit amet, consectetur adipiscing elit."
                        </blockquote>
                        <div class="flex items-center">
                          <img
                            class="w-16 h-16 rounded-full"
                            src="https://sandbox-tailwind-template.netlify.app/assets/img/avatars/te3.jpg"
                            alt="User"
                          />
                          <div class="ml-4">
                            <h5 class="text-base font-semibold">David Smith</h5>
                            <p class="text-sm text-gray-500">
                              Financial Advisor
                            </p>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="swiper-slide flex w-1/2">
                      <div class="bg-white shadow-lg rounded-lg p-6">
                        <blockquote class="text-gray-800 text-lg italic mb-4">
                          "Vestibulum id ligula porta felis euismod semper. Sed
                          posuere consectetur est at lobortis. Lorem ipsum dolor
                          sit amet, consectetur adipiscing elit."
                        </blockquote>
                        <div class="flex items-center">
                          <img
                            class="w-16 h-16 rounded-full"
                            src="https://sandbox-tailwind-template.netlify.app/assets/img/avatars/te4.jpg"
                            alt="User"
                          />
                          <div class="ml-4">
                            <h5 class="text-base font-semibold">Sophia Rose</h5>
                            <p class="text-sm text-gray-500">UX/UI Designer</p>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>

                <div class="swiper-pagination"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <div>
      <SalesFinance />
    </div>
  </div>
</template>

<style scoped>
.container {
  max-width: 1200px;
  margin: 0 auto;
}
</style>
