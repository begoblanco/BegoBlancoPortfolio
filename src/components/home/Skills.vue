<template>
    <div class="container mx-auto px-4">
        <div class="text-center">
          <h1 class="text-3xl font-bold text-pink-500">Skills</h1>
        </div>
        <div class="mt-8 grid grid-cols-1 md:grid-cols-3 gap-8 ">
          
          <div class="flex flex-col items-center px-6">
            <h2 class="text-xl font-semibold text-pink-400">Front-end</h2>
            <ul class="mt-4 space-y-2 list-disc list-outside text-gray-600">
              <li>Responsive Web Design</li>
              <li>UI/UX Design Principles</li>
              <li>DOM Manipulation & Event Handling</li>
              <li>Component-based Architecture (Vue 3)</li>
              <li>Client-Side Routing (Vue Router)</li>
              <li>Design Prototyping with Figma</li>
            </ul>
          </div>
          <div class="flex flex-col items-center px-6">
            <h2 class="text-xl font-semibold text-pink-400">Back-end</h2>
            <ul class="mt-4 space-y-2 list-disc list-outside text-gray-600">
              <li>RESTful API Design & Development</li>
              <li>Java Web Development (Spring Boot)</li>
              <li>Object-Oriented Programming (OOP) in Java</li>
              <li>SQL Queries</li>
              <li>Authentication & Authorization (JWT, OAuth)</li>
              <li>Docker Containerization</li>
              <li>Unit Testing (JUnit)</li>
              <li>API Testing (Postman)</li>
            </ul>
          </div>
          <div class="flex flex-col items-center px-6">
            <h2 class="text-xl font-semibold text-pink-400">Cybersecurity</h2>
            <ul class="mt-4 space-y-2 list-disc list-outside text-gray-600">
              <li>Security Auditing</li>
              <li>Network Security Analysis</li>
              <li>Linux Administration</li>
              <li>SQL Query Optimization</li>
              <li>Identifying and addressing vulnerabilities</li>
              <li>Documenting and handling incidents </li>
            </ul>
          </div>
        </div>
      </div>
</template>