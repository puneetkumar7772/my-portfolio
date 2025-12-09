<template>
    <nav class="w-full px-6 py-4 bg-[#0d0d0d] border-b border-gray-800 flex items-center justify-between">
        <div class="text-white text-xl font-bold tracking-wide">
            Puneet Kumar
        </div>

        <div class="flex items-center gap-4">

            <a href="/resume" target="_blank" class="flex items-center gap-1 text-gray-300 hover:text-white transition">
                Resume
                <ArrowTopRightOnSquareIcon class="w-4 h-4" />
            </a>
            <a href="https://www.linkedin.com/in/puneet-kumar-4a428426b/" target="_blank" class="flex items-center justify-center
         w-9 h-9 rounded-full
         bg-[#1a1a1a] border border-gray-700/40
         text-gray-300 hover:text-white
         hover:bg-[#242424]
         transition-all duration-200">
                <LinkedinIcon class="w-4 h-4" />
            </a>
            <a href="https://github.com/puneetkumar7772" target="_blank" class="flex items-center justify-center
         w-9 h-9 rounded-full
         bg-[#1a1a1a] border border-gray-700/40
         text-gray-300 hover:text-white
         hover:bg-[#242424]
         transition-all duration-200">
                <GithubIcon class="w-4 h-4" />
            </a>

        </div>
    </nav>
</template>

<script setup>
import { ArrowTopRightOnSquareIcon } from "@heroicons/vue/24/outline"
import { GithubIcon, LinkedinIcon } from "lucide-vue-next"
</script>
