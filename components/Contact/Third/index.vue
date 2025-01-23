<template>
  <div class="w-full flex flex-col items-center justify-center mt-12 md:mt-20 p-4">
    <h1 class="text-[40px] font-bold text-gray-900 mb-2">Drop Us a Line</h1>
    <span class="text-[16px] text-gray-800 mb-4">Reach out to us from our contact form and we will get back to you shortly.</span>
    <form
      class="items-center justify-center md:px-16 px-8 py-8 w-full md:min-w-[1000px] max-w-2xl rounded-lg"
      @submit.prevent="handleSubmit"
    >
      <!-- First Name and Last Name -->
      <div class="flex flex-col md:flex-row md:space-x-6 space-y-4 md:space-y-0">
        <div class="w-full">
          <input
            type="text"
            id="first-name"
            v-model="form.firstName"
            placeholder="Enter your first name"
            class="w-full px-4 py-3 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500"
            required
          />
        </div>
        <div class="w-full">
          <input
            type="text"
            id="last-name"
            v-model="form.lastName"
            placeholder="Enter your last name"
            class="w-full px-4 py-3 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500"
            required
          />
        </div>
      </div>

      <!-- Email and Select Department -->
      <div class="flex flex-col md:flex-row md:space-x-6 space-y-4 md:space-y-0 mt-6">
        <div class="w-full">
          <input
            type="email"
            id="email"
            v-model="form.email"
            placeholder="Enter your email"
            class="w-full px-4 py-3 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500"
            required
          />
        </div>
        <div class="w-full">
          <select
            id="department"
            v-model="form.department"
            class="w-full px-4 py-3 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500"
            required
          >
            <option value="" disabled>Select a department</option>
            <option value="sales">Sales</option>
            <option value="support">Support</option>
            <option value="development">Development</option>
            <option value="marketing">Marketing</option>
          </select>
        </div>
      </div>

      <!-- Message -->
      <div class="mt-6">
        <textarea
          id="message"
          v-model="form.message"
          placeholder="Write your message here"
          class="w-full px-4 py-3 md:h-[150px] border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500"
          rows="4"
          required
        ></textarea>
      </div>

      <!-- Submit Button -->
      <div class="mt-6 text-center">
        <button
          type="submit"
          class=" bg-blue-500 text-white px-4 py-3 w-[200px] rounded-md hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-500 transition-all"
        >
          Submit
        </button>
      </div>
    </form>
  </div>
</template>

<script>
import { reactive } from "vue";

export default {
  setup() {
    const form = reactive({
      firstName: "",
      lastName: "",
      email: "",
      department: "",
      message: "",
    });

    const handleSubmit = () => {
      console.log("Form Submitted:", form);
      alert("Form submitted successfully!");
    };

    return { form, handleSubmit };
  },
};
</script>

<style >

</style>
