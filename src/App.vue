<template>
  <div :class="{ 'dark': dark }" class="min-h-screen bg-gray-100 dark:bg-gray-900 text-gray-900 dark:text-gray-200 transition-colors duration-300">
    <!-- Navbar with dark mode toggle -->
    <Navbar @toggle-dark="toggleDark" />

    <!-- Main sections -->
    <Hero />
    <About />
    <Projects />
    <Contact />
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'

import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Contact from './components/Contact.vue'

// Dark mode enabled by default
const dark = ref(true)

// Persist user preference
onMounted(() => {
  const saved = localStorage.getItem('darkMode')
  if (saved !== null) dark.value = saved === 'true'
})

const toggleDark = () => {
  dark.value = !dark.value
  localStorage.setItem('darkMode', dark.value)
}
</script>
