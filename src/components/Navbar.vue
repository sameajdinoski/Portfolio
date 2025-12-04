<template>
  <nav class="flex justify-between items-center p-4 bg-white dark:bg-gray-800 text-black dark:text-white shadow-md transition-colors duration-300">
    <!-- Logo / Brand -->
    <div class="text-xl font-bold">My Portfolio</div>

    <!-- Links -->
    <ul class="hidden md:flex space-x-6">
      <li><a href="#hero" class="hover:text-blue-500">Home</a></li>
      <li><a href="#about" class="hover:text-blue-500">About</a></li>
      <li><a href="#projects" class="hover:text-blue-500">Projects</a></li>
      <li><a href="#contact" class="hover:text-blue-500">Contact</a></li>
    </ul>

    <!-- Dark Mode Toggle Button -->
    <button
      @click="$emit('toggle-dark')"
      class="ml-4 px-3 py-1 rounded-md border border-gray-500 dark:border-gray-300 hover:bg-gray-200 dark:hover:bg-gray-700 transition-colors duration-200"
    >
      Toggle Dark/Light
    </button>
  </nav>
</template>

<script setup>
// Nothing needed here, toggle emits to App.vue
</script>
