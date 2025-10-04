<template>
  <div class="min-h-screen bg-white">
    <!-- Hero Section -->
    <section class="relative min-h-screen flex items-center">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 w-full">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
          <!-- Contenido de texto -->
          <div class="order-2 lg:order-1">
            <div class="inline-block mb-4">
              <span class="text-sm font-medium text-gray-500 uppercase tracking-wider">
                Ingeniero en Software | Desarrollo & Redes
              </span>
            </div>

            <h1 class="text-5xl md:text-6xl font-bold text-gray-900 leading-tight mb-6">
              Hola, soy<br />
              <span class="text-indigo-600">Alberto Castrejón Hernández</span>
            </h1>

            <p class="text-lg text-gray-600 leading-relaxed mb-8 max-w-xl">
              Soy egresado de <strong>Ingeniería en Software</strong>, con experiencia
              en <strong>desarrollo de plataformas web</strong> y también en
              <strong>redes, soporte técnico y administración de sistemas Linux</strong>.
              Mi perfil combina programación y tecnología de la información para aportar
              valor en diferentes áreas.
            </p>

            <div class="flex flex-wrap gap-4">
              <router-link to="/projects"
                class="inline-flex items-center px-6 py-3 bg-gray-900 text-white font-medium rounded hover:bg-gray-800 transition-colors duration-200">
                Ver Proyectos
                <svg class="w-5 h-5 ml-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3">
                  </path>
                </svg>
              </router-link>

              <router-link to="/contact"
                class="inline-flex items-center px-6 py-3 border-2 border-gray-900 text-gray-900 font-medium rounded hover:bg-gray-50 transition-colors duration-200">
                Contacto
              </router-link>
            </div>
          </div>

          <!-- Imagen/Visual -->
          <div class="order-1 lg:order-2">
            <div class="relative">
              <div class="relative z-10 rounded-lg overflow-hidden shadow-2xl bg-gray-100 aspect-square">
                <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?w=800&h=800&fit=crop"
                  alt="Workspace desarrollo" class="w-full h-full object-cover" />
              </div>
              <div class="absolute -bottom-6 -right-6 w-full h-full border-2 border-gray-900 rounded-lg -z-0"></div>
            </div>
          </div>
        </div>
      </div>

      <!-- Indicador de scroll -->
      <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2 hidden md:block">
        <div class="flex flex-col items-center animate-bounce">
          <span class="text-xs text-gray-500 mb-2">Scroll</span>
          <svg class="w-6 h-6 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
          </svg>
        </div>
      </div>
    </section>

    <!-- Sección: Sobre Mí -->
    <section class="py-24 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
          <!-- Imagen -->
          <div class="order-2 lg:order-1">
            <div class="relative rounded-lg overflow-hidden shadow-lg bg-gray-200 aspect-video">
              <img src="https://images.unsplash.com/photo-1517694712202-14dd9538aa97?w=800&h=600&fit=crop"
                alt="Coding workspace" class="w-full h-full object-cover" />
            </div>
          </div>

          <!-- Contenido -->
          <div class="order-1 lg:order-2">
            <h2 class="text-4xl font-bold text-gray-900 mb-6">Sobre Mí</h2>
            <div class="space-y-4 text-gray-600 leading-relaxed">
              <p>
                Soy egresado de <strong>Ingeniería en Software</strong> con
                conocimientos en
                <strong>redes, telecomunicaciones y servidores Linux</strong>. Tengo
                experiencia práctica en configuración de routers y switches
                (<strong>CCNA</strong>).
              </p>
              <p>
                He desarrollado proyectos utilizando <strong>tecnologías modernas como Node.js, Express, Vue, React y
                  MySQL</strong>, además de explorar el uso de <strong>inteligencia artificial</strong> para crear
                soluciones innovadoras y automatizadas.
              </p>

              <p>
                Mi objetivo es seguir creciendo tanto en el área de
                <strong>desarrollo de software</strong> como en la de
                <strong>infraestructura y soporte técnico</strong>, aplicando buenas
                prácticas y creando soluciones que impacten de forma positiva.
              </p>
            </div>

            <div class="mt-8">
              <router-link to="/about" class="inline-flex items-center text-gray-900 font-medium hover:underline">
                Conoce más sobre mí
                <svg class="w-5 h-5 ml-2" fill="none" í stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3">
                  </path>
                </svg>
              </router-link>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Sección: Habilidades -->
    <section class="py-24 bg-white">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold text-gray-900 mb-4">Habilidades Técnicas</h2>
          <p class="text-lg text-gray-600 max-w-2xl mx-auto">
            Áreas en las que tengo experiencia y sigo desarrollándome profesionalmente
          </p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <!-- Desarrollo -->
          <div class="bg-gray-50 rounded-lg p-8 border border-gray-200">
            <h3 class="text-xl font-semibold text-gray-900 mb-4 flex items-center gap-2">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-indigo-600" fill="none" viewBox="0 0 24 24"
                stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
              </svg>
              Desarrollo
            </h3>
            <ul class="space-y-3 text-gray-600">
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-indigo-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M12.316 3.051a1 1 0 01.633 1.265l-4 12a1 1 0 11-1.898-.632l4-12a1 1 0 011.265-.633zM5.707 6.293a1 1 0 010 1.414L3.414 10l2.293 2.293a1 1 0 11-1.414 1.414l-3-3a1 1 0 010-1.414l3-3a1 1 0 011.414 0zm8.586 0a1 1 0 011.414 0l3 3a1 1 0 010 1.414l-3 3a1 1 0 11-1.414-1.414L16.586 10l-2.293-2.293a1 1 0 010-1.414z"
                    clip-rule="evenodd" />
                </svg>
                HTML5, CSS3, JavaScript (ES6+)
              </li>
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-indigo-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M3 5a2 2 0 012-2h10a2 2 0 012 2v8a2 2 0 01-2 2H5a2 2 0 01-2-2V5zm2 0v8h10V5H5z"
                    clip-rule="evenodd" />
                </svg>
                Vue.js & React
              </li>
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-indigo-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M2 5a2 2 0 012-2h12a2 2 0 012 2v10a2 2 0 01-2 2H4a2 2 0 01-2-2V5zm3.293 1.293a1 1 0 011.414 0l3 3a1 1 0 010 1.414l-3 3a1 1 0 01-1.414-1.414L7.586 10 5.293 7.707a1 1 0 010-1.414zM12 6a1 1 0 011 1v6a1 1 0 11-2 0V7a1 1 0 011-1z"
                    clip-rule="evenodd" />
                </svg>
                Node.js & Express
              </li>
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-indigo-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M4 4a2 2 0 00-2 2v8a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2H4zm2 2h8v2H6V6zm0 3h8v2H6V9zm0 3h8v2H6v-2z"
                    clip-rule="evenodd" />
                </svg>
                MySQL & MongoDB
              </li>
            </ul>
          </div>

          <!-- Redes & Sistemas -->
          <div class="bg-gray-50 rounded-lg p-8 border border-gray-200">
            <h3 class="text-xl font-semibold text-gray-900 mb-4 flex items-center gap-2">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-600" fill="none" viewBox="0 0 24 24"
                stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round"
                  d="M5 12h14M5 12a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v4a2 2 0 01-2 2M5 12a2 2 0 00-2 2v4a2 2 0 002 2h14a2 2 0 002-2v-4a2 2 0 00-2-2" />
              </svg>
              Redes & Sistemas
            </h3>
            <ul class="space-y-3 text-gray-600">
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M2 5a2 2 0 012-2h12a2 2 0 012 2v2a2 2 0 01-2 2H4a2 2 0 01-2-2V5zm3 1h10v1H5V6zm-3 5a2 2 0 012-2h12a2 2 0 012 2v2a2 2 0 01-2 2H4a2 2 0 01-2-2v-2zm3 1h10v1H5v-1z"
                    clip-rule="evenodd" />
                </svg>
                CCNA: configuración de routers y switches
              </li>
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z"
                    clip-rule="evenodd" />
                </svg>
                Soporte técnico y diagnóstico
              </li>
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M2 5a2 2 0 012-2h12a2 2 0 012 2v10a2 2 0 01-2 2H4a2 2 0 01-2-2V5zm3 1h10v8H5V6z"
                    clip-rule="evenodd" />
                </svg>
                Administración de servidores Linux
              </li>
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-green-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M3 5a2 2 0 012-2h10a2 2 0 012 2v8a2 2 0 01-2 2H5a2 2 0 01-2-2V5zm11 1H6v8h8V6z"
                    clip-rule="evenodd" />
                </svg>
                Despliegue básico en entornos virtualizados
              </li>
            </ul>
          </div>

          <!-- Herramientas -->
          <div class="bg-gray-50 rounded-lg p-8 border border-gray-200">
            <h3 class="text-xl font-semibold text-gray-900 mb-4 flex items-center gap-2">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-yellow-600" fill="none" viewBox="0 0 24 24"
                stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round"
                  d="M11 5.882V19.24a1.76 1.76 0 01-3.417.592l-2.147-6.15M18 13a3 3 0 100-6M5.436 13.683A4.001 4.001 0 017 6h1.832c4.1 0 7.625-1.234 9.168-3v14c-1.543-1.766-5.067-3-9.168-3H7a3.988 3.988 0 01-1.564-.317z" />
              </svg>
              Herramientas
            </h3>
            <ul class="space-y-3 text-gray-600">
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-yellow-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
                    clip-rule="evenodd" />
                </svg>
                Git & GitHub
              </li>
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-yellow-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M3 3a2 2 0 012-2h10a2 2 0 012 2v14a2 2 0 01-2 2H5a2 2 0 01-2-2V3zm2 2v10h10V5H5z"
                    clip-rule="evenodd" />
                </svg>
                VS Code
              </li>
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-yellow-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M3 5a2 2 0 012-2h10a2 2 0 012 2v10a2 2 0 01-2 2H5a2 2 0 01-2-2V5zm2 2h10v8H5V7z"
                    clip-rule="evenodd" />
                </svg>
                Figma
              </li>
              <li class="flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-yellow-500" viewBox="0 0 20 20"
                  fill="currentColor">
                  <path fill-rule="evenodd"
                    d="M5 3a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2V5a2 2 0 00-2-2H5zm0 2h10v10H5V5z"
                    clip-rule="evenodd" />
                </svg>
                Docker básico
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- Sección: Proyectos Destacados -->
    <section class="py-24 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-16">
          <h2 class="text-4xl font-bold text-gray-900 mb-4">Proyectos Destacados</h2>
          <p class="text-lg text-gray-600 max-w-2xl mx-auto">
            Algunos de los proyectos en los que he trabajado
          </p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
          <!-- Proyecto 1 -->
          <div
            class="bg-white rounded-lg overflow-hidden border border-gray-200 hover:shadow-lg transition-shadow duration-300 flex flex-col">
            <div class="aspect-video bg-gray-200">
              <img :src="LoginPEE" alt="Login PEE" class="w-full h-full object-cover" />
            </div>
            <div class="p-6 flex-1 flex flex-col">
              <h3 class="text-xl font-semibold text-gray-900 mb-3">
                Plataforma Estancias y Estadías
              </h3>
              <p class="text-gray-600 mb-4 leading-relaxed flex-1">
                Sistema web desarrollado en <strong>React, Express</strong> y <strong>MySQL</strong> para gestionar
                estancias académicas y estadías profesionales, con panel de administración
                y seguimiento de estudiantes.
              </p>
              <router-link to="/projects"
                class="mt-auto inline-block text-center border border-gray-900 text-gray-900 px-3 py-2 rounded hover:bg-gray-900 hover:text-white transition-colors duration-200 text-sm">
                Ver Proyecto
              </router-link>
            </div>
          </div>

          <!-- Proyecto 2 -->
          <div
            class="bg-white rounded-lg overflow-hidden border border-gray-200 hover:shadow-lg transition-shadow duration-300 flex flex-col">
            <div class="aspect-video bg-gray-200">
              <img :src="RedTalento" alt="Bolsa de Trabajo UPQROO" class="w-full h-full object-cover" />
            </div>
            <div class="p-6 flex-1 flex flex-col">
              <h3 class="text-xl font-semibold text-gray-900 mb-3">
                Bolsa de Trabajo UPQROO
              </h3>
              <p class="text-gray-600 mb-4 leading-relaxed flex-1">
                Portal de empleo para la UPQROO desarrollado con
                <strong>Next.js, Node.js </strong> y <strong> MySQL</strong>. Permite a estudiantes y
                egresados consultar ofertas laborales y postularse directamente.
              </p>
              <router-link to="/projects"
                class="mt-auto inline-block text-center border border-gray-900 text-gray-900 px-3 py-2 rounded hover:bg-gray-900 hover:text-white transition-colors duration-200 text-sm">
                Ver Proyecto
              </router-link>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Call to Action -->
    <section class="py-24 bg-gray-900">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-4xl font-bold text-white mb-6">¿Hablamos?</h2>
        <p class="text-xl text-gray-300 mb-8 max-w-2xl mx-auto">
          Me gusta trabajar en equipo y aprender de cada experiencia. Estoy buscando nuevas oportunidades como
          <strong>Frontend Developer</strong>, <strong>Fullstack Junior</strong> o en
          <strong>redes y soporte técnico</strong>. Si tienes una idea o proyecto en mente, estaré encantado de
          conocerlo.
        </p>

        <router-link to="/contact"
          class="inline-flex items-center px-8 py-4 bg-white text-gray-900 font-medium rounded hover:bg-gray-100 transition-colors duration-200">
          Enviar mensaje
        </router-link>
      </div>
    </section>
  </div>
</template>

<script>
import LoginPEE from "../assets/LoginPEE.png";
import RedTalento from "../assets/RedTalento.png";

export default {
  name: "Home",
  data() {
    return {
      LoginPEE,
      RedTalento,
    };
  },
};
</script>

<style scoped>
@keyframes bounce {

  0%,
  100% {
    transform: translateY(0);
  }

  50% {
    transform: translateY(-10px);
  }
}

.animate-bounce {
  animation: bounce 2s infinite;
}
</style>
