<script setup>
import PortfolioItem from "@/components/PortfolioItem.vue";

const projects = [
  {
    id: 1,
    title: "Laika",
    description: "A virtual assistant that, through the use of Large Language Models (LLM), is capable of providing answers to the user based on a database. Additionally, it features chat, notes, and a calendar for event scheduling.",
    image: "https://i.imgur.com/49I1AjR.jpeg",
    link: "https://github.com/begoblanco/Laika-Project-Front",
    
  },
  {
    id: 2,
    title: "FunkoShop",
    description: "Online e-commerce platform built as part of a student team project. It allows users to browse and purchase a wide range of Funko Pop products.",
    image: "https://camo.githubusercontent.com/e9a4c124b614b062feb5e68635c1a979df2dc829b1a79ffa5926fe330b5751c3/68747470733a2f2f692e696d6775722e636f6d2f52736f475678342e706e67",
    link: "https://github.com/begoblanco/P3-Digital-Academy-Project-FunkoShop-Frontend",
  },
 
];
</script>

<template>
  <div class="container mx-auto p-4">
    <div class="container mx-auto">
      <h2 class="text-3xl font-bold text-center mb-8 text-pink-500">Projects</h2>
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
