  <script setup>
  defineProps({
    project: {
      type: Object,
      required: true,
    },
  });
  </script>
<template>
    <div class="bg-white shadow-md rounded-lg overflow-hidden">
      <img :src="project.image" alt="Project Image" class="w-full h-48 object-cover">
      <div class="p-4">
        <h2 class="text-lg font-bold">{{ project.title }}</h2>
        <p class="text-gray-600">{{ project.description }}</p>
      </div>
    </div>
  </template>
  