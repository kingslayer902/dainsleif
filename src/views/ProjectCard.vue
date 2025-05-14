<template>
  <div class="bg-white rounded-2xl shadow-md p-5 hover:shadow-2xl hover:scale-105 transition duration-300 ease-in-out transform">
    <div class="mb-3">
      <img :src="project.image" class="rounded-md w-full h-auto" alt="Thumbnail Project" />
    </div>
    <h2 class="text-xl font-bold text-gray-800">{{ project.name }}</h2>
    <p class="text-gray-600 text-sm mt-2 mb-4">{{ project.description }}</p>
    <a :href="project.link" target="_blank" class="text-indigo-600 font-semibold hover:underline">
      🔗 Lihat Proyek di GitHub
    </a>
  </div>
</template>

<script>
export default {
  props: {
    project: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
/* Tambahkan sedikit animasi atau efek */
.hover\:scale-105:hover {
  transform: scale(1.05); /* Membesarkan sedikit card saat dihover */
}
</style>
