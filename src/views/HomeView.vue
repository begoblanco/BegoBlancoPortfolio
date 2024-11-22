<script setup>
import AboutMe from "@/components/home/AboutMe.vue";
import TechStack from "@/components/home/TechStack.vue";
import Skills from "@/components/home/Skills.vue";
import Projects from "@/components/home/Projects.vue";
</script>

<template>
  <div>
    <section id="about" class="bg-gray-200 py-12">
      <AboutMe />
    </section>
      
    <section id="techstack" class="py-12 border-t-8 border-pink-300">
      <TechStack />
    </section>

    <section id="skills" class="py-12  border-t-8 border-pink-300">
      <Skills />
    </section>

    <section id="projects" class="py-12  border-t-8 border-pink-300">
      <Projects />
    </section>

    <section id="contact" class="py-12  border-t-8 border-pink-300">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold text-center mb-8">Contact me</h2>
      </div>
    </section>
  </div>
</template>
