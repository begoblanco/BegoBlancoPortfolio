<script setup>
import PortfolioItem from "@/components/PortfolioItem.vue";

const projects = [
  {
    id: 1,
    title: "Proyecto 1",
    description: "Descripción breve del proyecto 1.",
    image: "https://via.placeholder.com/300",
  },
  {
    id: 2,
    title: "Proyecto 2",
    description: "Descripción breve del proyecto 2.",
    image: "https://via.placeholder.com/300",
  },
  // Agrega más proyectos aquí
];
</script>
<template>
  <div>
    <section id="about" class="bg-gray-100 py-12">
      <div class="container mx-auto">
        <!-- Título -->
        <div class="text-center">
          <h1 class="text-3xl font-bold">About me</h1>
        </div>
        <!-- Contenido -->
        <div class="mt-8 flex flex-col md:flex-row items-center">
          <!-- Texto -->
          <div class="md:w-1/2 px-4 text-center md:text-left">
            <p class="text-gray-600">
              Hi! My name is Bego and I'm a Full-Stack Web Developer!
            </p>
            <p class="text-gray-600">
              I specialize in both Front-end and Back-end development. I enjoy
              logic and problem-solving. I can work both in a team and
              individually, always giving my best and trying to help in any way
              I can.
            </p>
            <p class="text-gray-600">
              Other interests of mine include learning new languages, microbiology,
              electronics, robotics, 3D modeling, art and design!
            </p>
            <p class="text-gray-600">｡･:*:･ﾟ★,｡･:*:･ﾟ☆｡｡･:*:･ﾟ★,｡･:*:･ﾟ☆｡</p>
          </div>
          <!-- GIF -->
          <!-- src="https://media1.tenor.com/m/w3APLkMuTX0AAAAC/computer-work.gif" -->
          <div class="md:w-1/2 px-4 flex justify-center mt-8 md:mt-0">
            <img
               src="https://media1.tenor.com/m/tdLMhEHtcZ8AAAAd/rina-tennoji.gif"
              alt="about me gif"
              class=" h-64 object-cover rounded-lg shadow-lg"
            />
          </div>
        </div>
      </div>
    </section>

    <section id="techstack" class="py-12">
      <div class="container mx-auto">
        <!-- Título -->
        <div class="text-center">
          <h1 class="text-3xl font-bold">Tech Stack</h1>
        </div>
        <!-- Contenido -->
        <div class="mt-8 grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
          <!-- Front-end -->
          <div>
            <h2 class="text-xl font-semibold">Front-end</h2>
            <ul class="mt-4 space-y-2">
              <li>HTML5</li>
              <li>CSS3</li>
              <li>JavaScript</li>
              <li>Vue 3</li>
              <li>Bootstrap</li>
              <li>Tailwind CSS</li>
            </ul>
          </div>
          <!-- Back-end -->
          <div>
            <h2 class="text-xl font-semibold">Back-end</h2>
            <ul class="mt-4 space-y-2">
              <li>Java</li>
              <li>Python</li>
              <li>SpringBoot</li>
            </ul>
          </div>
          <!-- Others -->
          <div>
            <h2 class="text-xl font-semibold">Others</h2>
            <ul class="mt-4 space-y-2">
              <li>Docker</li>
              <li>Postman</li>
              <li>MySQL</li>
              <li>Figma</li>
              <li>Arduino</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <section id="skills" class="py-12">
      <div class="container mx-auto">
        <!-- Título -->
        <div class="text-center">
          <h1 class="text-3xl font-bold">Skills</h1>
        </div>
        <!-- Contenido -->
        <div class="mt-8 grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
          <!-- Front-end -->
          <div>
            <h2 class="text-xl font-semibold">Front-end</h2>
            <ul class="mt-4 space-y-2">
              <li>HTML5</li>
              <li>CSS3</li>
              <li>JavaScript</li>
              <li>Vue 3</li>
              <li>Bootstrap</li>
              <li>Tailwind CSS</li>
            </ul>
          </div>
          <!-- Back-end -->
          <div>
            <h2 class="text-xl font-semibold">Back-end</h2>
            <ul class="mt-4 space-y-2">
              <li>Java</li>
              <li>Python</li>
              <li>SpringBoot</li>
            </ul>
          </div>
          <!-- Others -->
          <div>
            <h2 class="text-xl font-semibold">Others</h2>
            <ul class="mt-4 space-y-2">
              <li>Docker</li>
              <li>Postman</li>
              <li>MySQL</li>
              <li>Figma</li>
              <li>Arduino</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <section id="portfolio" class="py-12">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold text-center mb-8">Projects</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <PortfolioItem
            v-for="project in projects"
            :key="project.id"
            :project="project"
          />
        </div>
      </div>
    </section>

    <section id="contact" class="py-12">
      <div class="container mx-auto">
        <h2 class="text-3xl font-bold text-center mb-8">Contact me</h2>
      </div>
    </section>
  </div>
</template>
