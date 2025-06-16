<script setup lang="ts">
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import About from './views/About.vue'
import Projects from './views/Projects.vue'
import Lab from './views/Lab.vue'
import Contact from './views/Contact.vue'
</script>

<template>
  <div class="h-screen w-screen snap-y snap-mandatory scroll-smooth overflow-y-scroll">
    <Header class="sticky top-0"/>
    <main class="">
      <About />
      <Projects />
      <Lab />
      <Contact />
    </main>
  </div>
</template>