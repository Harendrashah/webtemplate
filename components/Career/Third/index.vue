<template>
  <div>
    <!-- Job Positioning Section -->
    <div class="flex flex-col items-center justify-start mt-16 space-y-4">
      <!-- Job Positioning Title and Description -->
      <span class="text-xl font-semibold">Job Positioning</span>
      <span class="text-[36px] text-center max-w-[866px]">
        We’re always searching for amazing people to join our team. Take a look
        at our current openings.
      </span>

      <div class="flex flex-col">
        <div class="flex flex-col md:flex-row gap-4 mt-6">
          <!-- Position Select -->
          <div class="flex flex-col w-full md:w-[300px]">
            <label for="position" class="text-lg font-medium mb-2">Position</label>
            <select
              id="position"
              class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
            >
              <option value="developer">Developer</option>
              <option value="designer">Designer</option>
              <option value="manager">Manager</option>
              <option value="qa">QA</option>
            </select>
          </div>

          <!-- Type Select -->
          <div class="flex flex-col w-full md:w-[300px]">
            <label for="type" class="text-lg font-medium mb-2">Type</label>
            <select
              id="type"
              class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
            >
              <option value="full-time">Full-Time</option>
              <option value="part-time">Part-Time</option>
              <option value="internship">Internship</option>
            </select>
          </div>

          <!-- Location Select -->
          <div class="flex flex-col w-full md:w-[300px]">
            <label for="location" class="text-lg font-medium mb-2">Location</label>
            <select
              id="location"
              class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
            >
              <option value="remote">Remote</option>
              <option value="on-site">On-site</option>
              <option value="hybrid">Hybrid</option>
            </select>
          </div>
        </div>

        <!-- Designer Section -->
        <div class="flex flex-col mt-[65px]">
          <h2 class="text-[22px]">Designer</h2>
          <CareerInfoCard
            v-for="(item, index) in designerData"
            :key="index"
            :card="item"
          />
        </div>

        <!-- Developer Section -->
        <div class="flex flex-col mt-[65px] space-y-6">
          <h2 class="text-[22px] font-semibold text-gray-800">Developer</h2>
          <CareerInfoCard
            v-for="(item, index) in developerData"
            :key="index"
            :card="item"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const designerData = [
 
{ name: "Ram Sh", time: "Full-time", location: "Remote" }, { name: "Name2", time: "Part-time", location: "Remote" }, { name: "Shyam", time: "Full-time", location: "Remote" },
];

const developerData = [
{ name: "Hari", time: "Full-time", location: "Remote" }, { name: "Prashad sth", time: "Part-time", location: "Remote" }, { name: "name1", time: "Full-time", location: "Remote" },
];
</script>

<style scoped></style>
