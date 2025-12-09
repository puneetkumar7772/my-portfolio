<template>
  <section class="w-full min-h-screen text-white flex items-center">
    <div class="max-w-7xl mx-auto w-full px-8 py-12 flex flex-col lg:flex-row justify-between">

      <!-- LEFT CONTENT -->
      <div class="max-w-xl space-y-6">

        <!-- Title -->
        <h1 class="text-5xl font-bold leading-tight">
          Hi, I am <span class="text-purple-400">Puneet Kumar</span>
          <br />
          <span class="text-5xl font-extrabold text-blue-400">Frontend Developer</span>
        </h1>

        <!-- Paragraph -->
        <p class="text-gray-300 text-lg leading-relaxed">
          I build fast, modern, user-friendly web applications using Vue, React, Tailwind CSS,
          Node.js, and more. I focus on writing clean code, beautiful UI, and smooth user experiences.
        </p>

        <!-- SOCIAL ICONS -->
        <div class="flex gap-4 pt-2">

          <!-- Portfolio -->
          <a 
            href="#" 
            target="_blank" 
            class="flex items-center justify-center w-12 h-12 rounded-full 
                   border border-gray-600/40 bg-[#1a1a1a] text-gray-300 
                   hover:bg-[#2d2d2d] hover:text-white transition-all duration-200"
          >
            <GlobeIcon class="w-6 h-6" />
          </a>

          <!-- GitHub -->
          <a 
            href="https://github.com/puneetkumar7772" 
            target="_blank" 
            class="flex items-center justify-center w-12 h-12 rounded-full 
                   border border-gray-600/40 bg-[#1a1a1a] text-gray-300 
                   hover:bg-[#2d2d2d] hover:text-white transition-all duration-200"
          >
            <GithubIcon class="w-6 h-6" />
          </a>

          <!-- LinkedIn -->
          <a 
            href="https://www.linkedin.com/in/puneet-kumar-4a428426b/" 
            target="_blank" 
            class="flex items-center justify-center w-12 h-12 rounded-full 
                   border border-gray-600/40 bg-[#1a1a1a] text-gray-300 
                   hover:bg-[#2d2d2d] hover:text-white transition-all duration-200"
          >
            <LinkedinIcon class="w-6 h-6" />
          </a>

          <!-- Email -->
          <a 
            href="mailto:test@gmail.com" 
            class="flex items-center justify-center w-12 h-12 rounded-full 
                   border border-gray-600/40 bg-[#1a1a1a] text-gray-300 
                   hover:bg-[#2d2d2d] hover:text-white transition-all duration-200"
          >
            <MailIcon class="w-6 h-6" />
          </a>

        </div>

        <!-- Button -->
        <a
          href="#"
          class="inline-block mt-4 px-8 py-3 bg-blue-600 hover:bg-blue-700 rounded-lg 
                 text-lg font-semibold shadow-md transition"
        >
          Resume
        </a>
      </div>

      <!-- RIGHT ILLUSTRATION -->
    <div class="mt-12 lg:mt-0 lg:ml-10">
  <img
    src="https://images.unsplash.com/photo-1518770660439-4636190af475?auto=format&fit=crop&w=900&q=80"
    alt="developer working at desk"
    class="w-[450px] rounded-xl shadow-lg opacity-95"
  />
</div>
    </div>
  </section>
</template>

<script setup>
import { GithubIcon, LinkedinIcon, MailIcon, GlobeIcon } from "lucide-vue-next";
</script>
