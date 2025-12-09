<template>
     <ScrollReveal>
  <section class="w-full max-w-5xl mx-auto px-8 py-16 text-gray-200">
    
    <!-- Heading -->
    <div class="text-center mb-10">
      <h2 class="text-4xl font-bold mb-3 bg-gradient-to-r from-purple-400 to-blue-400 bg-clip-text text-transparent">
        Contact Me
      </h2>
      <p class="text-gray-400 text-lg">
        Feel free to reach out for collaborations, project discussions, or just to say hello.
      </p>
    </div>

    <!-- Form Container -->
    <div class="bg-[#161616]/80 backdrop-blur-md border border-gray-700/40 
                rounded-2xl p-8 shadow-xl">

      <form @submit.prevent="submitForm" class="space-y-6">

        <!-- Name -->
        <div>
          <label class="block text-gray-300 mb-2 font-medium">Name</label>
          <input
            v-model="form.name"
            type="text"
            placeholder="Enter your name"
            class="w-full px-4 py-3 rounded-lg bg-[#1f1f1f] border border-gray-700 
                   text-gray-200 placeholder-gray-500 
                   focus:ring-2 focus:ring-purple-500 focus:border-purple-500 
                   transition-all outline-none"
          />
        </div>

        <!-- Email -->
        <div>
          <label class="block text-gray-300 mb-2 font-medium">Email</label>
          <input
            v-model="form.email"
            type="email"
            placeholder="Enter your email"
            class="w-full px-4 py-3 rounded-lg bg-[#1f1f1f] border border-gray-700 
                   text-gray-200 placeholder-gray-500 
                   focus:ring-2 focus:ring-purple-500 focus:border-purple-500 
                   transition-all outline-none"
          />
        </div>

        <!-- Message -->
        <div>
          <label class="block text-gray-300 mb-2 font-medium">Message</label>
          <textarea
            v-model="form.message"
            rows="5"
            placeholder="Enter your message"
            class="w-full px-4 py-3 rounded-lg bg-[#1f1f1f] border border-gray-700 
                   text-gray-200 placeholder-gray-500 
                   focus:ring-2 focus:ring-purple-500 focus:border-purple-500 
                   transition-all outline-none resize-none"
          ></textarea>
        </div>

        <!-- Submit Button -->
        <div class="">
          <button
            type="submit"
            class="px-8 py-3 bg-purple-600 hover:bg-purple-700 rounded-lg 
                   text-lg font-semibold shadow-md transition-all duration-300
                   hover:shadow-purple-500/20 hover:-translate-y-1 cursor-pointer"
          >
            Submit
          </button>
        </div>

      </form>

    </div>

  </section>
  </ScrollReveal>
</template>

<script setup>
    import ScrollReveal from "./ScrollReveal.vue";
import { reactive } from "vue";

const form = reactive({
  name: "",
  email: "",
  message: "",
});

const submitForm = () => {
  console.log("Form Submitted:", form);
  alert("Message sent successfully!");
};
</script>
