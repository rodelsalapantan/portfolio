<template>
  <TopContact />

  <main class="p-4">
    <Hero />
    <Portfolio />
    <AboutMe />
    <Skills />
    <Education />
  </main>

  <Footer />
</template>

<script setup>
import { onMounted } from 'vue'
import Hero from '@/components/Hero.vue'
import TopContact from '@/components/TopContact.vue'
import Portfolio from '@/components/Portfolio.vue'
import AboutMe from '@/components/AboutMe.vue';
import Skills from '@/components/Skills.vue';
import Education from '@/components/Education.vue';
import Footer from '@/components/Footer.vue';

import AOS from 'aos';

onMounted(() => {
  AOS.init({
    duration: 1000,
  });
})
</script>
