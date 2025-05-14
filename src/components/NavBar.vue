<template>
  <nav class="p-4 flex gap-6">
    <router-link to="/" class="hover:text-yellow-300 font-bold" active-class="text-blue-400 font-bold">Home</router-link>
    <router-link to="/about" class="hover:text-yellow-300 font-bold">Tentang</router-link>
    <router-link to="/project" class="hover:text-yellow-300 font-bold">Project</router-link>

      <!-- Ini untuk ke WhatsApp -->
    <a
      href="https://wa.me/6281234567890"
      target="_blank"
      class="hover:text-green-400 font-bold" 
    >
      Contact Me
    </a>


   
  </nav>
</template>
