<template>
  <div id="app" class="min-h-screen bg-white">
    <!-- Header/Navegación -->
    <header class="fixed w-full top-0 z-50 bg-white/95 backdrop-blur-sm border-b border-gray-200 transition-all duration-300">
      <nav
        class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-6"
        aria-label="Menú principal"
      >
        <div class="flex justify-between items-center">
          <!-- Logo / Iniciales -->
          <router-link
            to="/"
            class="text-xl font-bold text-gray-900 tracking-tight hover:text-indigo-600 transition-all duration-200 transform hover:scale-105"
          >
            ACH
          </router-link>

          <!-- Menú en desktop -->
          <div class="hidden md:flex space-x-8">
            <router-link
              to="/"
              class="text-gray-600 hover:text-gray-900 font-normal transition-colors duration-200 relative group"
            >
              Inicio
              <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-indigo-600 transition-all duration-300 group-hover:w-full"></span>
            </router-link>
            <router-link
              to="/about"
              class="text-gray-600 hover:text-gray-900 font-normal transition-colors duration-200 relative group"
            >
              Acerca
              <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-indigo-600 transition-all duration-300 group-hover:w-full"></span>
            </router-link>
            <router-link
              to="/projects"
              class="text-gray-600 hover:text-gray-900 font-normal transition-colors duration-200 relative group"
            >
              Proyectos
              <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-indigo-600 transition-all duration-300 group-hover:w-full"></span>
            </router-link>
            <router-link
              to="/contact"
              class="text-gray-600 hover:text-gray-900 font-normal transition-colors duration-200 relative group"
            >
              Contacto
              <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-indigo-600 transition-all duration-300 group-hover:w-full"></span>
            </router-link>
          </div>

          <!-- Botón del menú móvil -->
          <button
            @click="isMenuOpen = !isMenuOpen"
            class="md:hidden text-gray-700 hover:text-gray-900 transition-colors duration-200 p-2 rounded-lg hover:bg-gray-100"
            aria-label="Abrir menú móvil"
          >
            <svg
              v-if="!isMenuOpen"
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              ></path>
            </svg>
            <svg
              v-else
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              ></path>
            </svg>
          </button>
        </div>

        <!-- Menú móvil desplegable -->
        <transition name="slide-fade">
          <div
            v-if="isMenuOpen"
            class="md:hidden mt-4 space-y-2 bg-white border border-gray-200 rounded-lg p-4 shadow-lg"
          >
            <router-link
              to="/"
              class="block text-gray-700 hover:text-gray-900 hover:bg-gray-50 font-medium py-2 px-3 rounded transition-colors duration-200"
              @click="isMenuOpen = false"
            >
              Inicio
            </router-link>
            <router-link
              to="/about"
              class="block text-gray-700 hover:text-gray-900 hover:bg-gray-50 font-medium py-2 px-3 rounded transition-colors duration-200"
              @click="isMenuOpen = false"
            >
              Acerca
            </router-link>
            <router-link
              to="/projects"
              class="block text-gray-700 hover:text-gray-900 hover:bg-gray-50 font-medium py-2 px-3 rounded transition-colors duration-200"
              @click="isMenuOpen = false"
            >
              Proyectos
            </router-link>
            <router-link
              to="/contact"
              class="block text-gray-700 hover:text-gray-900 hover:bg-gray-50 font-medium py-2 px-3 rounded transition-colors duration-200"
              @click="isMenuOpen = false"
            >
              Contacto
            </router-link>
          </div>
        </transition>
      </nav>
    </header>

    <!-- Contenido de la vista actual -->
    <main class="pt-24 min-h-screen">
      <router-view />
    </main>

    <!-- Footer -->
    <footer class="bg-gray-50 border-t border-gray-200">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
        <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
          <!-- Columna 1 -->
          <div>
            <h3 class="text-lg font-semibold text-gray-900 mb-3">
              Ingeniero de Software
            </h3>
            <p class="text-gray-600 text-sm leading-relaxed">
              Especializado en soluciones digitales, desarrollo web y soporte técnico.
            </p>
          </div>

          <!-- Columna 2 -->
          <div>
            <h4
              class="text-sm font-semibold text-gray-900 mb-3 uppercase tracking-wider"
            >
              Navegación
            </h4>
            <ul class="space-y-2">
              <li>
                <router-link
                  to="/"
                  class="text-sm text-gray-600 hover:text-gray-900 transition-colors duration-200 inline-flex items-center group"
                >
                  <span class="mr-2 transition-transform duration-200 group-hover:translate-x-1">→</span>
                  Inicio
                </router-link>
              </li>
              <li>
                <router-link
                  to="/about"
                  class="text-sm text-gray-600 hover:text-gray-900 transition-colors duration-200 inline-flex items-center group"
                >
                  <span class="mr-2 transition-transform duration-200 group-hover:translate-x-1">→</span>
                  Acerca de mí
                </router-link>
              </li>
              <li>
                <router-link
                  to="/projects"
                  class="text-sm text-gray-600 hover:text-gray-900 transition-colors duration-200 inline-flex items-center group"
                >
                  <span class="mr-2 transition-transform duration-200 group-hover:translate-x-1">→</span>
                  Proyectos
                </router-link>
              </li>
              <li>
                <router-link
                  to="/contact"
                  class="text-sm text-gray-600 hover:text-gray-900 transition-colors duration-200 inline-flex items-center group"
                >
                  <span class="mr-2 transition-transform duration-200 group-hover:translate-x-1">→</span>
                  Contacto
                </router-link>
              </li>
            </ul>
          </div>

          <!-- Columna 3 - Conecta -->
          <div>
            <h4
              class="text-sm font-semibold text-gray-900 mb-3 uppercase tracking-wider"
            >
              Conecta
            </h4>
            <div class="flex space-x-4">
              <!-- GitHub -->
              <a
                href="https://github.com/AlbertoCastre"
                target="_blank"
                rel="noopener noreferrer"
                class="w-10 h-10 bg-gray-100 rounded-lg flex items-center justify-center hover:bg-gray-900 transition-all duration-200 transform hover:scale-110 group"
                aria-label="GitHub"
              >
                <svg
                  class="w-5 h-5 text-gray-700 group-hover:text-white transition-colors duration-200"
                  fill="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"
                  />
                </svg>
              </a>

              <!-- LinkedIn -->
              <a
                href="https://linkedin.com/in/alberto-castrejon-4609982b7"
                target="_blank"
                rel="noopener noreferrer"
                class="w-10 h-10 bg-gray-100 rounded-lg flex items-center justify-center hover:bg-blue-600 transition-all duration-200 transform hover:scale-110 group"
                aria-label="LinkedIn"
              >
                <svg
                  class="w-5 h-5 text-gray-700 group-hover:text-white transition-colors duration-200"
                  fill="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"
                  />
                </svg>
              </a>

              <!-- Email / Contacto -->
              <router-link
                to="/contact"
                class="w-10 h-10 bg-gray-100 rounded-lg flex items-center justify-center hover:bg-indigo-600 transition-all duration-200 transform hover:scale-110 group"
                aria-label="Contacto"
              >
                <svg
                  class="w-5 h-5 text-gray-700 group-hover:text-white transition-colors duration-200"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
                  />
                </svg>
              </router-link>
            </div>
            
            <p class="text-xs text-gray-500 mt-4">
              ¿Quieres colaborar? ¡Escríbeme!
            </p>
          </div>
        </div>

        <div class="border-t border-gray-200 mt-12 pt-8">
          <p class="text-center text-sm text-gray-500">
            &copy; 2025 Alberto Castrejón Hernández. Todos los derechos reservados.
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      isMenuOpen: false,
    };
  },
  watch: {
    $route() {
      this.isMenuOpen = false;
    }
  }
};
</script>

<style>
/* Router link activo con línea inferior */
.router-link-active {
  color: #111827 !important;
  font-weight: 500;
}

.router-link-active span {
  width: 100%;
  background-color: #4f46e5;
}

/* Animación del menú móvil */
.slide-fade-enter-active {
  transition: all 0.3s ease;
}

.slide-fade-leave-active {
  transition: all 0.2s ease;
}

.slide-fade-enter-from {
  transform: translateY(-10px);
  opacity: 0;
}

.slide-fade-leave-to {
  transform: translateY(-10px);
  opacity: 0;
}

/* Backdrop blur fallback */
@supports not (backdrop-filter: blur(12px)) {
  header {
    background-color: white;
  }
}

/* Smooth scroll global */
html {
  scroll-behavior: smooth;
}

/* Estilos para la barra de scroll */
::-webkit-scrollbar {
  width: 10px;
}

::-webkit-scrollbar-track {
  background: #f1f1f1;
}

::-webkit-scrollbar-thumb {
  background: #888;
  border-radius: 5px;
}

::-webkit-scrollbar-thumb:hover {
  background: #555;
}
</style>