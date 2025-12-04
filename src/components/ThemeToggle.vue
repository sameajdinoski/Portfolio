<template>
  <button @click="toggleTheme" class="px-4 py-2 bg-gray-300 dark:bg-gray-700 rounded">
    Toggle Theme
  </button>
</template>

<script setup>
const toggleTheme = () => {
  document.documentElement.classList.toggle('dark')
}
</script>
