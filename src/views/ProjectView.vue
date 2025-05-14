<template>
  <main class="min-h-screen bg-gray-100 py-10 px-4">
    <h1 class="text-3xl font-bold text-center mb-8 text-gray-800">My Projects</h1>

    <div class="grid gap-6 md:grid-cols-2 lg:grid-cols-3 max-w-7xl mx-auto">
      <div
        v-for="(project, index) in projects"
        :key="index"
        class="bg-white rounded-xl shadow-md p-5 hover:bg-blue-50 transition-all duration-300"
      >
        <img
          :src="project.image"
          :alt="project.name"
          class="rounded-md mb-4 w-full h-40 object-cover"
        />
        <h2 class="text-xl font-semibold text-gray-800 mb-2">{{ project.name }}</h2>
        <p class="text-gray-600 text-sm mb-4">{{ project.description }}</p>
        <a
          @click.prevent="showToast(project.name)"
          class="inline-block bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700 transition cursor-pointer"
        >
          Lihat Proyek
        </a>
      </div>
    </div>
  </main>
</template>

<script>
import axios from 'axios';
import { toast } from 'vue3-toastify';
import 'vue3-toastify/dist/index.css';

export default {
  name: 'ProjectView',
  data() {
    return {
      projects: []
    };
  },
  mounted() {
    axios.get('/projects.json')
      .then(response => {
        this.projects = response.data;
      })
      .catch(error => {
        console.error('Gagal memuat data project:', error);
      });
  },
  methods: {
    showToast(projectName) {
      toast.info(`Proyek "${projectName}" masih dalam tahap pengembangan!`, {
        position: "top-right",
        autoClose: 3000, // Menampilkan notifikasi selama 3 detik
      });
    }
  }
};
</script>
