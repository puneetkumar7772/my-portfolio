<script setup>
import NavBar from "./components/NavBar.vue";
// import SideBar from "./components/SideBar.vue";
import HomePage from "./components/HomePage.vue";
import ProfileSummary from "./components/ProfileSummary.vue";
import TechnologiesSection from "./components/TechnologiesSection.vue";
import ContactForm from "./components/ContactForm.vue";
</script>

<template>
  <div class="flex flex-col h-screen bg-[#0d0d0d] text-white">

    <NavBar />
    <div class=" bg-gradient-to-b from-[#0e0e0e] to-[#1a1a1a]">
      <ScrollReveal>
    <HomePage />
  </ScrollReveal>

  <ScrollReveal>
    <ProfileSummary />
  </ScrollReveal>
    <ScrollReveal>
    <TechnologiesSection />
  </ScrollReveal>
  <ScrollReveal>
    <ContactForm />
  </ScrollReveal>
  
    </div>
  </div>
</template>