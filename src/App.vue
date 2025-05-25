<script setup>
// import HelloWorld from './components/HelloWorld.vue'
// import TheWelcome from './components/TheWelcome.vue'
document.body.classList.toggle(
  'dark',
  localStorage.theme === 'dark' ||
  (!('theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches),
)
</script>

<template>
  <main class="flex min-h-screen dark:bg-neutral-900 dark:text-neutral-200">
    <h1 class="bg-blue-200 text-black dark:bg-blue-700 dark:text-neutral-300">Main</h1>
  </main>
</template>

<style scoped></style>
