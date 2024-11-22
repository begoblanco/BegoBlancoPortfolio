<script setup>
import PortfolioItem from "@/components/PortfolioItem.vue";

const projects = [
  {
    id: 1,
    title: "Laika",
    description: "A virtual assistant that, through the use of Large Language Models (LLM), is capable of providing answers to the user based on a database. Additionally, it features chat, notes, and a calendar for event scheduling.",
    image: "https://private-user-images.githubusercontent.com/168825653/374137042-594b9db5-5bf9-4d3c-9629-f0ffa4aa4018.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzIyODAwMzEsIm5iZiI6MTczMjI3OTczMSwicGF0aCI6Ii8xNjg4MjU2NTMvMzc0MTM3MDQyLTU5NGI5ZGI1LTViZjktNGQzYy05NjI5LWYwZmZhNGFhNDAxOC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQxMTIyJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MTEyMlQxMjQ4NTFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0wN2M1YTk5NmNhY2M5N2ZlMDQzYzRkZTY3NzFkYjQwZDJhMTI1ZDI3ZDBhODEwNzBjOWI3M2E2OTZkZjNjZmQwJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.ZGmQAKNwQH0y0H9k1-Ks-gNKby_iDsKvvDUnWvMj7Yo",
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
