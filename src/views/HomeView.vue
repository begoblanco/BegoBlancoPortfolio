<script setup>
import AboutMe from "@/components/home/AboutMe.vue";
import TechStack from "@/components/home/TechStack.vue";
import Skills from "@/components/home/Skills.vue";
import Projects from "@/components/home/Projects.vue";
import ContactMe from "@/components/home/ContactMe.vue";
</script>

<template>
  <div>
    <section id="about" class="bg-pink-100 py-12">
      <AboutMe />
    </section>

    <section id="techstack" class="py-12 border-t-8 bg-gray-100 border-pink-300">
      <TechStack />
    </section>

    <section id="skills" class="py-12 border-t-8 bg-gray-100 border-pink-300">
      <Skills />
    </section>

    <section id="projects" class="py-12 border-t-8 bg-gray-100 border-pink-300">
      <Projects />
    </section>

    <section id="contact" class="py-12  bg-pink-400">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold text-center mb-8 text-white">Contact me 💌​</h2>
        <ContactMe />
      </div>
    </section>
  </div>
</template>
