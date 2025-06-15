<script setup lang="ts">
import Header from './components/Header.vue'
import About from './views/About.vue'
import Projects from './views/Projects.vue'
import Lab from './views/Lab.vue'
import Contact from './views/Contact.vue'
</script>

<template>
  <div class="app">
    <Header />
    <main>
      <About />
      <Projects />
      <Lab />
      <Contact />
    </main>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style scoped>
main {
  max-width: 800px;
  margin: 2rem auto;
  padding: 1rem;
}
</style>
