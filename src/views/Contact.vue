<script setup>
  import Footer from '../components/Footer.vue'
</script>

<!-- <template>
  <section id="contact" class="min-h-screen w-screen snap-start grid grid-rows-[1fr_auto]">
    <div class="h-full grid place-items-center">
      <h2 class="text-3xl font-bold mb-4">Contact Me</h2>
      <p class="text-gray-700">Placeholder text about who I am and what I do.</p>
    </div>
    <Footer />
  </section>
</template> -->

<template>
  <section
    id="contact"
    class="h-screen flex items-center justify-center px-4"
  >
    <div class="grid grid-cols-4 grid-rows-2 gap-4 w-full">
      <div class="col-start-2 row-start-1 self-end justify-self-center border">
        <h2 class="text-4xl sm:text-5xl md:text-6xl font-bold mb-4">Let's get in touch,</h2>
      </div>
      
      <div class="col-start-3 row-span-2 border">
        <p>
                      Lorem ipsum dolor sit amet consectetur adipiscing elit. Quisque faucibus ex sapien vitae pellentesque sem placerat. In id cursus mi pretium tellus duis convallis. Tempus leo eu aenean sed diam urna tempor. Pulvinar vivamus fringilla lacus nec metus bibendum egestas. Iaculis massa nisl malesuada lacinia integer nunc posuere. Ut hendrerit semper vel class aptent taciti sociosqu. Ad litora torquent per conubia nostra inceptos himenaeos.
            Lorem ipsum dolor sit amet consectetur adipiscing elit. Quisque faucibus ex sapien vitae pellentesque sem placerat. In id cursus mi pretium tellus duis convallis. Tempus leo eu aenean sed diam urna tempor. Pulvinar vivamus fringilla lacus nec metus bibendum egestas. Iaculis massa nisl malesuada lacinia integer nunc posuere. Ut hendrerit semper vel class aptent taciti sociosqu. Ad litora torquent per conubia nostra inceptos himenaeos.

        </p>
      </div>
      
      <div class="col-start-2 row-start-2 border">

      </div>
      
    </div>

  </section>
  <Footer class="bottom-0 left-0 snap-end"/>
</template>