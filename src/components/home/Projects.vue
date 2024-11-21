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
  <div class="container mx-auto">
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
  </div>
</template>