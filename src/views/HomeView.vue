<template>
  <main class="min-h-screen bg-white py-10 px-4">
    <!-- Hero Section -->
    <section class="text-center bg-gradient-to-br from-blue-100 to-blue-300 py-20 px-5  rounded-xl shadow mb-10">
      <h1 class="text-4xl font-bold text-gray-800 mb-4">Selamat Datang di Portofolio Saya 🎯</h1>
      <p class="text-lg text-gray-700 mb-6">
        Saya seorang pengembang web yang berfokus pada pembuatan project kreatif dan fungsional. 🚀
      </p>
      <router-link
        to="/project"
        class="inline-block bg-blue-600 text-white px-6 py-3 rounded-lg hover:bg-blue-700 hover:scale-105 transition-all shadow"
      >
        Lihat Proyek
      </router-link>
    </section>

    <!-- About Section -->
    <section class="text-center bg-white border border-gray-200 shadow-md rounded-xl p-6 mb-12">
      <h2 class="text-2xl font-semibold text-gray-800 mb-2">Tentang Saya 💡</h2>
      <p class="text-gray-600 text-md">
        Saya adalah developer Aplikasi dan Web dengan menggunakan Vue dan Tailwind. Website ini adalah tempat saya berbagi proyek-proyek yang saya kerjakan dan kembangkan.
      </p>
    </section>

    <!-- Skill Section (Optional) -->
    <section class="text-center">
      <h3 class="text-2xl font-semibold text-gray-800 mb-6">Keahlian Saya 🧠</h3>
      <div class="flex justify-center gap-6 mb-12">
        <div class="bg-gray-100 text-black p-6 rounded-lg shadow-lg hover:shadow-xl transform hover:scale-105 transition-all">
          <h4 class="text-xl font-semibold">Vue.js</h4>
          <p class="text-gray-600">Mengembangkan aplikasi web dengan Vue.js dan Vue Router.</p>
        </div>
        <div class="bg-gray-100 text-black p-6 rounded-lg shadow-lg hover:shadow-xl transform hover:scale-105 transition-all">
          <h4 class="text-xl font-semibold">Tailwind CSS</h4>
          <p class="text-gray-600">Desain antarmuka menggunakan Tailwind CSS yang responsif dan elegan.</p>
        </div>
      </div>
    </section>
  </main>
</template>

<script setup>
// Tidak ada script khusus untuk bagian ini
</script>

<style scoped>
/* Opsional: jika ingin menambah styling khusus di sini */
</style>
