<template>
  <div class="bg-[#ffffff] w-[100%] h-[full] mb-[100px] overflow-hidden">
    <div class="px-[7rem]">
      <div class="flex flex-col justify-center items-center gap-5">
        <div class="font-sans font-bold text-[35px]">Projects</div>
        <div
          class="w-[470px] h-[70px] text-[25px] text-[#60697B] font-sans font-semibold"
        >
          Check out some of our awesome projects with creative ideas and great
          design.
        </div>
      </div>
      <div class="flex flex-wrap gap-[10px]">
        <div
          v-for="(project, index) in projects"
          :key="index"
          :class="[
            'relative w-full',
            { 'ml-[47rem]': index % 2 !== 0, 'ml-[1rem]': index % 2 === 0 },
          ]"
        >
          <div
            class="absolute top-0 left-0 flex items-center z-10 w-full h-[90%]"
            :class="{
              'ml-[27rem]': index % 2 === 0,
              'absolute left-[-15rem] mt-3': index % 2 !== 0,
            }"
          >
            <div
              class="bg-white border shadow-sm w-[450px] h-[250px] flex flex-col justify-center p-5 rounded-xl mt-[150px]"
            >
              <p
                class="text-blue-600 text-sm text-[17px] font-semibold uppercase"
              >
                {{ project.category }}
              </p>
              <h3 class="text-gray-800 text-[25px] font-bold mt-4">
                {{ project.title }}
              </h3>
              <p class="text-gray-600 text-[19px] mt-6 ml-1">
                {{ project.description }}
              </p>
              <a
                :href="project.link"
                class="text-blue-600 font-semibold hover:underline mt-3"
              >
                See Project →
              </a>
            </div>
          </div>

          <div
            class="relative flex justify-start items-center mt-[250px] w-full"
          >
            <img
              :src="project.image"
              alt="Project Image"
              class="w-[619px] rounded-xl h-[639px] object-cover"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const projects = ref([
  {
    category: "Cosmetic",
    title: "Cras Fermentum Sem",
    description:
      "Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.",
    image:
      "https://sandbox-tailwind-template.netlify.app/assets/img/photos/cs16.jpg",
    link: "#",
  },
  {
    category: "Cosmetic",
    title: "Cras Fermentum Sem",
    description:
      "Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.",
    image:
      "https://sandbox-tailwind-template.netlify.app/assets/img/photos/cs17.jpg",
    link: "#",
  },
  {
    category: "Cosmetic",
    title: "Cras Fermentum Sem",
    description:
      "Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.",
    image:
      "https://sandbox-tailwind-template.netlify.app/assets/img/photos/cs18.jpg",
    link: "#",
  },
  {
    category: "Cosmetic",
    title: "Cras Fermentum Sem",
    description:
      "Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.",
    image:
      "https://sandbox-tailwind-template.netlify.app/assets/img/photos/cs19.jpg",
    link: "#",
  },
  {
    category: "Cosmetic",
    title: "Cras Fermentum Sem",
    description:
      "Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.",
    image:
      "https://sandbox-tailwind-template.netlify.app/assets/img/photos/cs20.jpg",
    link: "#",
  },
  {
    category: "Cosmetic",
    title: "Cras Fermentum Sem",
    description:
      "Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.",
    image:
      "https://sandbox-tailwind-template.netlify.app/assets/img/photos/cs21.jpg",
    link: "#",
  },
  {
    category: "Cosmetic",
    title: "Cras Fermentum Sem",
    description:
      "Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.",
    image:
      "https://sandbox-tailwind-template.netlify.app/assets/img/photos/cs22.jpg",
    link: "#",
  },
]);
</script>

<style scoped>
/* .history-timeline {
  position: relative;
  margin: 50px auto;
  padding: 40px 0;
  width: 100%;
  height: 100%;
}

.history-list {
  height: 100%;
} */

/* .history-timeline::before {
  content: "";
  position: absolute;
  left: 13px;
  top: 0px;
  width: 2px;
  height: 100%;
  transform: translateX(-50%);
  background-color: #e0e0e0; 
} */

/* .history-timeline .history-list .history-item {
  list-style: none;
  position: relative;
  width: 80%;
  padding: 20px 40px;
} */

/* .history-timeline .history-list .history-item:nth-child(odd) {
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  text-align: left;
}

.history-timeline .history-list .history-item:nth-child(even) {
  margin-left: 10px;
  margin-top: -60px;
} */

/* .history-timeline .history-list .history-item::before {
  content: "";
  position: absolute;
  left: 50%;
  width: 16px;
  height: 16px;
  background-color: #e0e0e0; 
  border-radius: 50%;
  transform: translateX(-50%);
}

.history-timeline .history-list .history-item:hover::before {
  transform: scale(1.5);
} */

/* .time {
  display: inline-flex;
  font-weight: 400;
  font-size: 14px !important;
  margin-bottom: 15px !important;
  border-radius: 20px;
} */

/* h3 {
  font-weight: 400;
  line-height: 20px;
}

.history-timeline .history-list .history-item h2 {
  color: #999;
  line-height: 20px;
}

.history-timeline .history-list .history-item p {
  font-weight: 300;
} */
</style>
