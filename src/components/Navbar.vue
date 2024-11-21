<script>
import { ref } from "vue";

export default {
  setup() {
    const isMenuOpen = ref(false);

    const toggleMenu = () => {
      isMenuOpen.value = !isMenuOpen.value;
    };

    const closeMenu = () => {
      isMenuOpen.value = false;
    };

    return {
      isMenuOpen,
      toggleMenu,
      closeMenu,
    };
  },
};
</script>

<template>
  <nav class="bg-white border-gray-200 dark:bg-pink-400 sticky top-0">
    <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
      <a href="/" class="flex items-center space-x-3 rtl:space-x-reverse">
        <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">My Portfolio</span>
      </a>

      <!-- Botón del menú hamburguesa -->
      <button
        type="button"
        @click="toggleMenu"
        :aria-expanded="isMenuOpen"
        class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-white-500 rounded-lg md:hidden"
      >
        <span class="sr-only">Open main menu</span>
        <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
          <path stroke="white" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15" />
        </svg>
      </button>

      <!-- Menú desplegable -->
      <div
        :class="{'hidden': !isMenuOpen, 'block': isMenuOpen, 'md:block': true}"
        id="navbar-default"
        class="w-full md:w-auto"
      >
        <ul
          class="font-medium flex flex-col p-4 md:p-0 mt-4 rounded-lg md:flex-row md:space-x-8 rtl:space-x-reverse md:mt-0"
        >
          <li>
            <a
              href="#about"
              @click="closeMenu"
              class="block py-2 px-3 rounded md:p-0 dark:text-white dark:hover:bg-pink-500 dark:hover:text-white md:dark:hover:bg-transparent"
            >
              About me
            </a>
          </li>
          <li>
            <a
              href="#techstack"
              @click="closeMenu"
              class="block py-2 px-3 rounded md:p-0 dark:text-white dark:hover:bg-pink-500 dark:hover:text-white md:dark:hover:bg-transparent"
            >
              Tech Stack
            </a>
          </li>
          <li>
            <a
              href="#skills"
              @click="closeMenu"
              class="block py-2 px-3 rounded md:p-0 dark:text-white dark:hover:bg-pink-500 dark:hover:text-white md:dark:hover:bg-transparent"
            >
              Skills
            </a>
          </li>
          <li>
            <a
              href="#projects"
              @click="closeMenu"
              class="block py-2 px-3 rounded md:p-0 dark:text-white dark:hover:bg-pink-500 dark:hover:text-white md:dark:hover:bg-transparent"
            >
              Projects
            </a>
          </li>
          <li>
            <a
              href="#contact"
              @click="closeMenu"
              class="block py-2 px-3 rounded md:p-0 dark:text-white dark:hover:bg-pink-500 dark:hover:text-white md:dark:hover:bg-transparent"
            >
              Contact me
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
