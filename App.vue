<!-- App.vue -->
<template>
  <div class="min-h-screen bg-gradient-to-br from-emerald-300 to-pink-300 text-white">
    <header class="p-4 ">
      <Navbar />
    </header>

    <main class="p-8">
      <router-view />
    </main>

    <footer class="p-4 text-center text-gray-400">
      &copy; 2025 MyWebsite
    </footer>
  </div>

</template>


<script setup>
import Navbar from './components/Navbar.vue'
</script>