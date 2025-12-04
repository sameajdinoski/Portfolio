<template>
  <section
    id="contact"
    class="min-h-screen flex flex-col justify-center items-center text-center p-8 bg-gray-50 dark:bg-gray-900 text-gray-800 dark:text-gray-200 transition-colors duration-300"
  >
    <h2 class="text-4xl font-bold mb-8">Contact Me</h2>
    <p class="mb-6">
      You can reach me at 
      <a href="mailto:sameajdinoski@gmail.com" class="text-blue-500 hover:underline">sameajdinoski@gmail.com</a>
    </p>

    <form class="flex flex-col max-w-md w-full space-y-4">
      <input
        type="text"
        placeholder="Name"
        class="p-2 rounded border border-gray-400 dark:border-gray-600 bg-white dark:bg-gray-700 text-black dark:text-white"
      />
      <input
        type="email"
        placeholder="Email"
        class="p-2 rounded border border-gray-400 dark:border-gray-600 bg-white dark:bg-gray-700 text-black dark:text-white"
      />
      <textarea
        placeholder="Message"
        class="p-2 rounded border border-gray-400 dark:border-gray-600 bg-white dark:bg-gray-700 text-black dark:text-white"
      ></textarea>
      <button
        type="submit"
        class="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600 transition-colors duration-200"
      >
        Send Message
      </button>
    </form>
  </section>
</template>

<script setup></script>
