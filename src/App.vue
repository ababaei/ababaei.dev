<script setup lang="ts">
import Header from './components/Header.vue'
import About from './views/About.vue'
import Projects from './views/Projects.vue'
import Lab from './views/Lab.vue'
import Contact from './views/Contact.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div class="app">
    <Header />
    <main class="max-w-3xl mx-auto px-4 snap-y snap-mandatory scroll-smooth h-screen overflow-y-scroll">
      <About />
      <Projects />
      <Lab />
      <Contact />
    </main>
    <Footer />
  </div>
</template>