<template>
  <!-- <NuxtLayout name="terms-layout"> -->
  <div>
    <TitlePage />
    <div class="flex bg-[#FEFEFE] min-h-screen">
      <div class="w-[20%] sticky top-0 self-start">
        <SideBar />
      </div>
      <div class="ml-[10%] w-[80%]">
        <div class="">
          <section id="term" class="content-section">
            <div
              class="w-[75%] h-[100%] mt-[100px] flex flex-col justify-center items-center bg-white border rounded-lg"
            >
              <h1 class="text-[22px] font-sans font-bold mb-4 p-4">
                1. Terms and Conditions
              </h1>
              <div class="flex flex-col gap-4 p-9">
                <p class="text-[19px] font-sans">
                  Donec id elit non mi porta gravida at eget metus. Praesent
                  commodo cursus magna, vel scelerisque nisl consectetur et.
                  Cras mattis consectetur purus sit amet fermentum. Lorem ipsum
                  dolor sit amet, consectetur adipiscing elit. Nulla vitae elit
                  libero, a pharetra augue. Nullam quis risus eget urna mollis
                  ornare vel eu leo. Cras justo odio, dapibus ac facilisis in,
                  egestas eget quam.
                </p>
                <p class="text-[19px] font-sans">
                  Sed posuere consectetur est at lobortis. Maecenas faucibus
                  mollis interdum. Cum sociis natoque penatibus et magnis dis
                  parturient montes, nascetur ridiculus mus. Donec id elit non
                  mi porta gravida at eget metus. Cras justo odio, dapibus ac
                  facilisis in, egestas eget quam. Cum sociis natoque penatibus
                  et magnis dis parturient montes, nascetur ridiculus mus.
                </p>
                <p class="text-[19px] font-sans">
                  Nullam quis risus eget urna mollis ornare vel eu leo. Maecenas
                  sed diam eget risus varius blandit sit amet non magna.
                  Praesent commodo cursus magna, vel scelerisque nisl
                  consectetur et. Nullam id dolor id nibh ultricies vehicula ut
                  id elit. Donec ullamcorper nulla non metus auctor fringilla.
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam
                  porta sem malesuada magna mollis euismod. Praesent commodo
                  cursus magna, vel scelerisque nisl consectetur et. Nulla vitae
                  elit libero, a pharetra augue. Curabitur blandit tempus
                  porttitor. Cras justo odio, dapibus ac facilisis in, egestas
                  eget quam. Fusce dapibus, tellus ac cursus commodo, tortor
                  mauris condimentum nibh, ut fermentum massa justo sit amet
                  risus. Aenean eu leo quam. Pellentesque ornare sem.
                </p>
              </div>
              <ul class="list-disc mb-7 text-[17px] py-5 space-y-2">
                <li>Aenean eu leo quam ornare curabitur blandit tempus.</li>
                <li>Nullam quis risus eget urna mollis ornare donec elit.</li>
                <li>Etiam porta sem malesuada magna mollis euismod.</li>
                <li>Fermentum massa vivamus faucibus amet euismod.</li>
              </ul>
            </div>
          </section>
          <section id="privacy-policy" class="content-section">
            <div
              class="w-[75%] h-[100%] mt-[100px] justify-center items-center flex flex-col bg-white border rounded-lg"
            >
              <h1 class="text-[22px] font-sans font-bold mb-4 p-4">
                2. privacy Policy
              </h1>
              <div class="flex flex-col gap-4 p-9">
                <p class="text-[19px] font-sans">
                  Donec id elit non mi porta gravida at eget metus. Praesent
                  commodo cursus magna, vel scelerisque nisl consectetur et.
                  Cras mattis consectetur purus sit amet fermentum. Lorem ipsum
                  dolor sit amet, consectetur adipiscing elit. Nulla vitae elit
                  libero, a pharetra augue. Nullam quis risus eget urna mollis
                  ornare vel eu leo. Cras justo odio, dapibus ac facilisis in,
                  egestas eget quam.
                </p>
                <p class="text-[19px] font-sans">
                  Sed posuere consectetur est at lobortis. Maecenas faucibus
                  mollis interdum. Cum sociis natoque penatibus et magnis dis
                  parturient montes, nascetur ridiculus mus. Donec id elit non
                  mi porta gravida at eget metus. Cras justo odio, dapibus ac
                  facilisis in, egestas eget quam. Cum sociis natoque penatibus
                  et magnis dis parturient montes, nascetur ridiculus mus.
                </p>
                <ul class="list-disc py-5 space-y-2 text-[18px] px-4">
                  <li>Aenean eu leo quam ornare curabitur blandit tempus.</li>
                  <li>Nullam quis risus eget urna mollis ornare donec elit.</li>
                  <li>Etiam porta sem malesuada magna mollis euismod.</li>
                  <li>Fermentum massa vivamus faucibus amet euismod.</li>
                </ul>
                <p class="text-[19px] font-sans">
                  Nullam quis risus eget urna mollis ornare vel eu leo. Maecenas
                  sed diam eget risus varius blandit sit amet non magna.
                  Praesent commodo cursus magna, vel scelerisque nisl
                  consectetur et. Nullam id dolor id nibh ultricies vehicula ut
                  id elit. Donec ullamcorper nulla non metus auctor fringilla.
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam
                  porta sem malesuada magna mollis euismod. Praesent commodo
                  cursus magna, vel scelerisque nisl consectetur et. Nulla vitae
                  elit libero, a pharetra augue. Curabitur blandit tempus
                  porttitor. Cras justo odio, dapibus ac facilisis in, egestas
                  eget quam. Fusce dapibus, tellus ac cursus commodo, tortor
                  mauris condimentum nibh, ut fermentum massa justo sit amet
                  risus. Aenean eu leo quam. Pellentesque ornare sem.
                </p>
              </div>
            </div>
          </section>
          <section id="user-policy" class="content-section">
            <div
              class="w-[75%] h-[100%] mt-[100px] justify-center items-center flex flex-col bg-white border rounded-lg"
            >
              <h1 class="text-[22px] font-sans font-bold mb-4 p-4">
                3. user-Policy
              </h1>
              <div class="flex flex-col gap-4 p-9">
                <p class="text-[19px] font-sans">
                  Donec id elit non mi porta gravida at eget metus. Praesent
                  commodo cursus magna, vel scelerisque nisl consectetur et.
                  Cras mattis consectetur purus sit amet fermentum. Lorem ipsum
                  dolor sit amet, consectetur adipiscing elit. Nulla vitae elit
                  libero, a pharetra augue. Nullam quis risus eget urna mollis
                  ornare vel eu leo. Cras justo odio, dapibus ac facilisis in,
                  egestas eget quam.
                </p>
                <p class="text-[19px] font-sans">
                  Sed posuere consectetur est at lobortis. Maecenas faucibus
                  mollis interdum. Cum sociis natoque penatibus et magnis dis
                  parturient montes, nascetur ridiculus mus. Donec id elit non
                  mi porta gravida at eget metus. Cras justo odio, dapibus ac
                  facilisis in, egestas eget quam. Cum sociis natoque penatibus
                  et magnis dis parturient montes, nascetur ridiculus mus.
                </p>
                <!-- <ul class="list-disc py-5 space-y-2 text-[18px] px-4">
                <li>Aenean eu leo quam ornare curabitur blandit tempus.</li>
                <li>Nullam quis risus eget urna mollis ornare donec elit.</li>
                <li>Etiam porta sem malesuada magna mollis euismod.</li>
                <li>Fermentum massa vivamus faucibus amet euismod.</li>
              </ul> -->
                <p class="text-[19px] font-sans">
                  Nullam quis risus eget urna mollis ornare vel eu leo. Maecenas
                  sed diam eget risus varius blandit sit amet non magna.
                  Praesent commodo cursus magna, vel scelerisque nisl
                  consectetur et. Nullam id dolor id nibh ultricies vehicula ut
                  id elit. Donec ullamcorper nulla non metus auctor fringilla.
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam
                  porta sem malesuada magna mollis euismod. Praesent commodo
                  cursus magna, vel scelerisque nisl consectetur et. Nulla vitae
                  elit libero, a pharetra augue. Curabitur blandit tempus
                  porttitor. Cras justo odio, dapibus ac facilisis in, egestas
                  eget quam. Fusce dapibus, tellus ac cursus commodo, tortor
                  mauris condimentum nibh, ut fermentum massa justo sit amet
                  risus. Aenean eu leo quam. Pellentesque ornare sem.
                </p>
              </div>
            </div>
          </section>
          <section id="copyright" class="content-section">
            <div
              class="w-[75%] h-[100%] mt-[100px] justify-center items-center flex flex-col bg-white border rounded-lg"
            >
              <h1 class="text-[22px] font-sans font-bold mb-4 p-4">
                4. Copyrights
              </h1>
              <div class="flex flex-col gap-4 p-9">
                <p class="text-[19px] font-sans">
                  Donec id elit non mi porta gravida at eget metus. Praesent
                  commodo cursus magna, vel scelerisque nisl consectetur et.
                  Cras mattis consectetur purus sit amet fermentum. Lorem ipsum
                  dolor sit amet, consectetur adipiscing elit. Nulla vitae elit
                  libero, a pharetra augue. Nullam quis risus eget urna mollis
                  ornare vel eu leo. Cras justo odio, dapibus ac facilisis in,
                  egestas eget quam.
                </p>
                <p class="text-[19px] font-sans">
                  Sed posuere consectetur est at lobortis. Maecenas faucibus
                  mollis interdum. Cum sociis natoque penatibus et magnis dis
                  parturient montes, nascetur ridiculus mus. Donec id elit non
                  mi porta gravida at eget metus. Cras justo odio, dapibus ac
                  facilisis in, egestas eget quam. Cum sociis natoque penatibus
                  et magnis dis parturient montes, nascetur ridiculus mus.
                </p>
                <ul class="list-disc py-5 space-y-2 text-[18px] px-4">
                  <li>Aenean eu leo quam ornare curabitur blandit tempus.</li>
                  <li>Nullam quis risus eget urna mollis ornare donec elit.</li>
                  <li>Etiam porta sem malesuada magna mollis euismod.</li>
                  <li>Fermentum massa vivamus faucibus amet euismod.</li>
                </ul>
                <p class="text-[19px] font-sans">
                  Nullam quis risus eget urna mollis ornare vel eu leo. Maecenas
                  sed diam eget risus varius blandit sit amet non magna.
                  Praesent commodo cursus magna, vel scelerisque nisl
                  consectetur et. Nullam id dolor id nibh ultricies vehicula ut
                  id elit. Donec ullamcorper nulla non metus auctor fringilla.
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam
                  porta sem malesuada magna mollis euismod. Praesent commodo
                  cursus magna, vel scelerisque nisl consectetur et. Nulla vitae
                  elit libero, a pharetra augue. Curabitur blandit tempus
                  porttitor. Cras justo odio, dapibus ac facilisis in, egestas
                  eget quam. Fusce dapibus, tellus ac cursus commodo, tortor
                  mauris condimentum nibh, ut fermentum massa justo sit amet
                  risus. Aenean eu leo quam. Pellentesque ornare sem.
                </p>
              </div>
            </div>
          </section>
          <section id="Cookies" class="content-section">
            <div
              class="w-[75%] h-[100%] mt-[100px] justify-center items-center flex flex-col bg-white border rounded-lg"
            >
              <h1 class="text-[22px] font-sans font-bold mb-4 p-4">
                5. Cookies
              </h1>
              <div class="flex flex-col gap-4 p-9">
                <p class="text-[19px] font-sans">
                  Donec id elit non mi porta gravida at eget metus. Praesent
                  commodo cursus magna, vel scelerisque nisl consectetur et.
                  Cras mattis consectetur purus sit amet fermentum. Lorem ipsum
                  dolor sit amet, consectetur adipiscing elit. Nulla vitae elit
                  libero, a pharetra augue. Nullam quis risus eget urna mollis
                  ornare vel eu leo. Cras justo odio, dapibus ac facilisis in,
                  egestas eget quam.
                </p>
                <p class="text-[19px] font-sans">
                  Sed posuere consectetur est at lobortis. Maecenas faucibus
                  mollis interdum. Cum sociis natoque penatibus et magnis dis
                  parturient montes, nascetur ridiculus mus. Donec id elit non
                  mi porta gravida at eget metus. Cras justo odio, dapibus ac
                  facilisis in, egestas eget quam. Cum sociis natoque penatibus
                  et magnis dis parturient montes, nascetur ridiculus mus.
                </p>
                <ul class="list-disc py-5 space-y-2 text-[18px] px-4">
                  <li>Aenean eu leo quam ornare curabitur blandit tempus.</li>
                  <li>Nullam quis risus eget urna mollis ornare donec elit.</li>
                  <li>Etiam porta sem malesuada magna mollis euismod.</li>
                  <li>Fermentum massa vivamus faucibus amet euismod.</li>
                </ul>
                <p class="text-[19px] font-sans">
                  Nullam quis risus eget urna mollis ornare vel eu leo. Maecenas
                  sed diam eget risus varius blandit sit amet non magna.
                  Praesent commodo cursus magna, vel scelerisque nisl
                  consectetur et. Nullam id dolor id nibh ultricies vehicula ut
                  id elit. Donec ullamcorper nulla non metus auctor fringilla.
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam
                  porta sem malesuada magna mollis euismod. Praesent commodo
                  cursus magna, vel scelerisque nisl consectetur et. Nulla vitae
                  elit libero, a pharetra augue. Curabitur blandit tempus
                  porttitor. Cras justo odio, dapibus ac facilisis in, egestas
                  eget quam. Fusce dapibus, tellus ac cursus commodo, tortor
                  mauris condimentum nibh, ut fermentum massa justo sit amet
                  risus. Aenean eu leo quam. Pellentesque ornare sem.
                </p>
              </div>
            </div>
          </section>
          <section id="account-billing" class="content-section">
            <div
              class="w-[75%] h-[100%] mt-[100px] justify-center items-center flex flex-col bg-white border rounded-lg mb-[10.50rem]"
            >
              <h1 class="text-[22px] font-sans font-bold mb-4 p-4">
                6. Account & Billing
              </h1>
              <div class="flex flex-col gap-4 p-9">
                <p class="text-[19px] font-sans">
                  Donec id elit non mi porta gravida at eget metus. Praesent
                  commodo cursus magna, vel scelerisque nisl consectetur et.
                  Cras mattis consectetur purus sit amet fermentum. Lorem ipsum
                  dolor sit amet, consectetur adipiscing elit. Nulla vitae elit
                  libero, a pharetra augue. Nullam quis risus eget urna mollis
                  ornare vel eu leo. Cras justo odio, dapibus ac facilisis in,
                  egestas eget quam.
                </p>
                <p class="text-[19px] font-sans">
                  Sed posuere consectetur est at lobortis. Maecenas faucibus
                  mollis interdum. Cum sociis natoque penatibus et magnis dis
                  parturient montes, nascetur ridiculus mus. Donec id elit non
                  mi porta gravida at eget metus. Cras justo odio, dapibus ac
                  facilisis in, egestas eget quam. Cum sociis natoque penatibus
                  et magnis dis parturient montes, nascetur ridiculus mus.
                </p>
                <ul class="list-disc py-5 space-y-2 text-[18px] px-4">
                  <li>Aenean eu leo quam ornare curabitur blandit tempus.</li>
                  <li>Nullam quis risus eget urna mollis ornare donec elit.</li>
                  <li>Etiam porta sem malesuada magna mollis euismod.</li>
                  <li>Fermentum massa vivamus faucibus amet euismod.</li>
                </ul>
                <p class="text-[19px] font-sans">
                  Nullam quis risus eget urna mollis ornare vel eu leo. Maecenas
                  sed diam eget risus varius blandit sit amet non magna.
                  Praesent commodo cursus magna, vel scelerisque nisl
                  consectetur et. Nullam id dolor id nibh ultricies vehicula ut
                  id elit. Donec ullamcorper nulla non metus auctor fringilla.
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam
                  porta sem malesuada magna mollis euismod. Praesent commodo
                  cursus magna, vel scelerisque nisl consectetur et. Nulla vitae
                  elit libero, a pharetra augue. Curabitur blandit tempus
                  porttitor. Cras justo odio, dapibus ac facilisis in, egestas
                  eget quam. Fusce dapibus, tellus ac cursus commodo, tortor
                  mauris condimentum nibh, ut fermentum massa justo sit amet
                  risus. Aenean eu leo quam. Pellentesque ornare sem.
                </p>
              </div>
            </div>
          </section>
        </div>
      </div>
    </div>
  </div>
  <!-- </NuxtLayout> -->
</template>

<script setup>
import SideBar from "~/components/AppNav/SideBar.vue";
import TitlePage from "./TitlePage.vue";
</script>
<style>
.content-section {
  padding: 20px;
  margin-bottom: 50px;
}
</style>
