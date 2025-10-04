<template>
  <div class="min-h-screen bg-white">
    <!-- Header de la página -->
    <section class="py-20 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <h1 class="text-5xl font-bold text-gray-900 mb-6">Mis Proyectos</h1>
          <p class="text-xl text-gray-600 max-w-3xl mx-auto">
            Algunos de los proyectos más representativos en los que he trabajado, integrando desarrollo web, bases de datos y despliegue en servidores.
          </p>
        </div>
      </div>
    </section>
    <!-- Filtros -->
    <section class="py-8 bg-white border-b border-gray-200">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex flex-wrap justify-center gap-3">
          <button 
            @click="currentFilter = 'todos'"
            :class="currentFilter === 'todos' ? 'bg-gray-900 text-white' : 'bg-gray-100 text-gray-700 hover:bg-gray-200'"
            class="px-4 py-2 rounded font-medium transition-colors duration-200"
          >
            Todos
          </button>
          <button 
            @click="currentFilter = 'web'"
            :class="currentFilter === 'web' ? 'bg-gray-900 text-white' : 'bg-gray-100 text-gray-700 hover:bg-gray-200'"
            class="px-4 py-2 rounded font-medium transition-colors duration-200"
          >
            Aplicaciones Web
          </button>
          <button 
            @click="currentFilter = 'frontend'"
            :class="currentFilter === 'frontend' ? 'bg-gray-900 text-white' : 'bg-gray-100 text-gray-700 hover:bg-gray-200'"
            class="px-4 py-2 rounded font-medium transition-colors duration-200"
          >
            Frontend
          </button>
          <button 
            @click="currentFilter = 'fullstack'"
            :class="currentFilter === 'fullstack' ? 'bg-gray-900 text-white' : 'bg-gray-100 text-gray-700 hover:bg-gray-200'"
            class="px-4 py-2 rounded font-medium transition-colors duration-200"
          >
            Full Stack
          </button>
        </div>
      </div>
    </section>
    <!-- Grid de proyectos -->
    <section class="py-20 bg-white">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div v-if="filteredProjects.length === 0" class="text-center text-gray-600 py-12">
          No hay proyectos en esta categoría por ahora.
        </div>
        <div v-else class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-12">
          <div
            v-for="(project, index) in filteredProjects"
            :key="project.title"
            class="bg-white rounded-lg border border-gray-200 overflow-hidden hover:shadow-lg transition-shadow duration-300 relative"
          >
            <!-- Icono EN USO -->
            <div class="absolute top-4 right-4 px-3 py-1 bg-red-500 text-white text-sm font-bold rounded animate-heartbeat">
              EN USO
            </div>
            <!-- Carrusel de imágenes -->
            <div class="relative aspect-video bg-gray-100">
              <div class="relative h-full overflow-hidden">
                <img
                  :src="project.images[project.currentImageIndex]"
                  :alt="'Screenshot de ' + project.title"
                  class="w-full h-full object-cover transition-opacity duration-300"
                  loading="lazy"
                />
              </div>
              <!-- Controles del carrusel -->
              <div class="absolute inset-0 flex items-center justify-between px-4">
                <button
                  @click="previousImage(index)"
                  aria-label="Imagen anterior"
                  class="w-10 h-10 rounded-full bg-white/90 hover:bg-white flex items-center justify-center shadow-lg transition-colors duration-200"
                >
                  <svg class="w-5 h-5 text-gray-900" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"></path>
                  </svg>
                </button>
                <button
                  @click="nextImage(index)"
                  aria-label="Imagen siguiente"
                  class="w-10 h-10 rounded-full bg-white/90 hover:bg-white flex items-center justify-center shadow-lg transition-colors duration-200"
                >
                  <svg class="w-5 h-5 text-gray-900" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path>
                  </svg>
                </button>
              </div>
              <!-- Indicadores -->
              <div class="absolute bottom-4 left-1/2 transform -translate-x-1/2 flex space-x-2">
                <div
                  v-for="(img, imgIndex) in project.images"
                  :key="imgIndex"
                  :class="imgIndex === project.currentImageIndex ? 'bg-white' : 'bg-white/50'"
                  class="w-2 h-2 rounded-full transition-colors duration-200"
                ></div>
              </div>
            </div>
            <!-- Contenido -->
            <div class="p-8">
              <h3 class="text-2xl font-bold text-gray-900 mb-3">{{ project.title }}</h3>
              <p class="text-gray-600 mb-4 leading-relaxed">{{ project.description }}</p>
              <!-- Tecnologías -->
              <div class="flex flex-wrap gap-2 mb-6">
                <span
                  v-for="tech in project.technologies"
                  :key="tech"
                  class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded"
                >
                  {{ tech }}
                </span>
              </div>
              <!-- Botón Visitar Sitio -->
              <div class="flex space-x-4">
                <a
                  :href="project.demoLink"
                  target="_blank"
                  rel="noopener noreferrer"
                  class="inline-flex items-center px-4 py-2 border-2 border-gray-900 text-gray-900 rounded hover:bg-gray-50 transition-colors duration-200"
                >
                  <svg class="w-4 h-4 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14"></path>
                  </svg>
                  Visitar Sitio
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Call to action -->
    <section class="py-20 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-3xl font-bold text-gray-900 mb-4">¿Te interesa colaborar?</h2>
        <p class="text-gray-600 mb-8 max-w-2xl mx-auto">
          Siempre estoy abierto a nuevos proyectos y oportunidades. Si tienes una idea en mente, hablemos.
        </p>
        <router-link 
          to="/contact" 
          class="inline-flex items-center px-8 py-4 bg-gray-900 text-white font-medium rounded hover:bg-gray-800 transition-colors duration-200"
        >
          Contactar
          <svg class="w-5 h-5 ml-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path>
          </svg>
        </router-link>
      </div>
    </section>
  </div>
</template>

<script>
import LoginPEE from '../assets/LoginPEE.png';
import HomeEstudiante from '../assets/HomeEstudiante.png';
import HomeAdmin from '../assets/HomeAdmin.png';
import Empresas from '../assets/Empresas.png';
import RedTalento from '../assets/RedTalento.png';
import RedPerfil from '../assets/RedPerfil.png';
import RedCreditos from '../assets/RedCreditos.png';

export default {
  name: 'ProjectsView',
  data() {
    return {
      currentFilter: 'todos',
      projects: [
        {
          title: 'Plataforma Estancias y Estadías',
          description: 'Sistema integral para la gestión de estancias y estadías profesionales. Implementado con React, Express y MySQL, permite administrar alumnos, empresas y reportes desde un panel de control moderno. Participé en todo el proceso: diseño de la base de datos, desarrollo fullstack y despliegue en entorno de producción.',
          technologies: ['React', 'Express', 'MySQL', 'Node.js', 'Tailwind CSS'],
          images: [LoginPEE, HomeEstudiante, HomeAdmin, Empresas],
          currentImageIndex: 0,
          demoLink: 'http://gestionvinculacion.upqroo.edu.mx', 
          category: 'fullstack',
        },
        {
          title: 'Red Talento UPQROO',
          description: 'Portal universitario orientado al vínculo laboral de estudiantes y egresados. Desarrollado con Next.js, Node.js y MySQL. Desplegué la aplicación en servidores Linux (Ubuntu) de la universidad, configurando el entorno y dependencias necesarias para su funcionamiento estable.',
          technologies: ['Next.js', 'Node.js', 'MySQL', 'Ubuntu', 'Linux Server'],
          images: [RedTalento, RedPerfil, RedCreditos],
          currentImageIndex: 0,
          demoLink: 'http://redtalento.upqroo.edu.mx', 
          category: 'fullstack',
        },
      ],
    };
  },
  computed: {
    filteredProjects() {
      if (this.currentFilter === 'todos') {
        return this.projects;
      }
      return this.projects.filter(p => p.category === this.currentFilter);
    },
  },
  methods: {
    nextImage(index) {
      const project = this.projects.find(p => p.title === this.filteredProjects[index].title);
      project.currentImageIndex = (project.currentImageIndex + 1) % project.images.length;
    },
    previousImage(index) {
      const project = this.projects.find(p => p.title === this.filteredProjects[index].title);
      project.currentImageIndex = (project.currentImageIndex - 1 + project.images.length) % project.images.length;
    },
  },
};
</script>

<style scoped>
@keyframes heartbeat {
  0% {
    transform: scale(1);
    opacity: 1;
  }
  50% {
    transform: scale(1.1);
    opacity: 0.8;
  }
  100% {
    transform: scale(1);
    opacity: 1;
  }
}
.animate-heartbeat {
  animation: heartbeat 1.5s infinite;
}
</style>