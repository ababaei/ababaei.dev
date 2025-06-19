<script setup lang="ts">
import Header from './components/Header.vue'
import About from './views/About.vue'
import Projects from './views/Projects.vue'
import Lab from './views/Lab.vue'
import Contact from './views/Contact.vue'
</script>

<template>
  <Header class="fixed top-0 left-0 w-full h-16 bg-white z-50 shadow"/>
  <div class="h-screen w-screen snap-y snap-mandatory scroll-smooth overflow-y-scroll">
    <main>
      <About />
      <Projects />
      <Lab />
      <Contact />
    </main>
  </div>
</template>