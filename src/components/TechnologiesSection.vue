<template>
    <ScrollReveal>
  <section 
    class="relative w-full py-20 px-6 overflow-hidden 
           bg-gradient-to-b from-[#0e0e0e] to-[#1a1a1a] text-white">

    <!-- Background Blur Shapes -->
    <div class="absolute top-10 left-20 w-72 h-72 bg-purple-600/20 rounded-full blur-3xl"></div>
    <div class="absolute bottom-10 right-20 w-72 h-72 bg-blue-600/20 rounded-full blur-3xl"></div>

    <!-- Content Wrapper -->
    <div class="max-w-6xl mx-auto relative z-10">

      <!-- Title -->
      <h2 class="text-4xl font-bold text-center mb-4 
                 bg-gradient-to-r from-purple-400 to-blue-400 bg-clip-text text-transparent">
        Technologies & Tools
      </h2>

      <p class="text-center text-gray-400 text-lg mb-12">
        A snapshot of the technologies, tools, and frameworks I use to build scalable, modern web applications.
      </p>

      <!-- GRID OF CARDS -->
      <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-6">

        <div 
          v-for="tech in technologies" 
          :key="tech.name"
          class="bg-[#161616]/70 border border-gray-700/40 rounded-xl p-5 flex flex-col 
                 items-center justify-center text-center hover:-translate-y-2 
                 hover:border-purple-500 hover:shadow-lg hover:shadow-purple-500/20 
                 transition-all duration-300 backdrop-blur-md"
        >
          <img :src="tech.icon" class="w-12 h-12 mb-3" />
          <p class="text-gray-300 font-medium text-sm">{{ tech.name }}</p>
        </div>

      </div>

    </div>
  </section>
  </ScrollReveal>
</template>

<script setup>
    import ScrollReveal from "./ScrollReveal.vue";
const technologies = [
  { name: "HTML5", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" },
  { name: "CSS3", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" },
  { name: "SCSS", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/sass/sass-original.svg" },
  { name: "JavaScript", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" },
  { name: "TypeScript", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" },

  { name: "Vue.js", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg" },
  { name: "Nuxt.js", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nuxtjs/nuxtjs-original.svg" },
  { name: "AngularJS", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg" },
  { name: "React.js", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" },
  { name: "Node.js", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" },

  { name: "Express.js", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/express/express-original.svg" },
  { name: "REST APIs", icon: "https://cdn-icons-png.flaticon.com/512/1491/1491310.png" },

  { name: "Bootstrap", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bootstrap/bootstrap-original.svg" },
  { name: "Tailwind CSS", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tailwindcss/tailwindcss-plain.svg" },
  { name: "Angular Material", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg" },
  { name: "Vuetify", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuetify/vuetify-original.svg" },

  { name: "Git", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" },
//   { name: "GitHub", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg?color=white" },
  { name: "Netlify", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/netlify/netlify-original.svg" },
  { name: "Vercel", icon: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vercel/vercel-original.svg" },
  { name: "Render", icon: "https://cdn-icons-png.flaticon.com/512/5968/5968520.png" }
];
</script>
