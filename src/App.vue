<template>
  <div id="app" class="min-h-screen bg-white">
    <!-- Header/Navegación -->
    <header class="fixed w-full top-0 z-50 bg-white border-b border-gray-200">
      <nav
        class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-6"
        aria-label="Menú principal"
      >
        <div class="flex justify-between items-center">
          <!-- Logo / Iniciales (ahora redirige al home) -->
          <router-link
            to="/"
            class="text-xl font-semibold text-gray-900 tracking-tight hover:text-gray-700 transition-colors duration-200"
          >
            ACH
          </router-link>

          <!-- Menú en desktop -->
          <div class="hidden md:flex space-x-8">
            <router-link
              to="/"
              class="text-gray-600 hover:text-gray-900 font-normal transition-colors duration-200"
            >
              Inicio
            </router-link>
            <router-link
              to="/about"
              class="text-gray-600 hover:text-gray-900 font-normal transition-colors duration-200"
            >
              Acerca
            </router-link>
            <router-link
              to="/projects"
              class="text-gray-600 hover:text-gray-900 font-normal transition-colors duration-200"
            >
              Proyectos
            </router-link>
            <router-link
              to="/contact"
              class="text-gray-600 hover:text-gray-900 font-normal transition-colors duration-200"
            >
              Contacto
            </router-link>
          </div>

          <!-- Botón del menú móvil -->
          <button
            @click="isMenuOpen = !isMenuOpen"
            class="md:hidden text-gray-700"
            aria-label="Abrir menú móvil"
          >
            <svg
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
          </button>
        </div>

        <!-- Menú móvil desplegable -->
        <div
          v-if="isMenuOpen"
          class="md:hidden mt-4 space-y-2 bg-white border border-gray-200 rounded-lg p-4 shadow-sm"
        >
          <router-link
            to="/"
            class="block text-gray-700 hover:text-gray-900 font-medium"
            @click="isMenuOpen = false"
          >
            Inicio
          </router-link>
          <router-link
            to="/about"
            class="block text-gray-700 hover:text-gray-900 font-medium"
            @click="isMenuOpen = false"
          >
            Acerca
          </router-link>
          <router-link
            to="/projects"
            class="block text-gray-700 hover:text-gray-900 font-medium"
            @click="isMenuOpen = false"
          >
            Proyectos
          </router-link>
          <router-link
            to="/contact"
            class="block text-gray-700 hover:text-gray-900 font-medium"
            @click="isMenuOpen = false"
          >
            Contacto
          </router-link>
        </div>
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
                  class="text-sm text-gray-600 hover:text-gray-900 transition-colors"
                >
                  Inicio
                </router-link>
              </li>
              <li>
                <router-link
                  to="/about"
                  class="text-sm text-gray-600 hover:text-gray-900 transition-colors"
                >
                  Acerca de mí
                </router-link>
              </li>
              <li>
                <router-link
                  to="/projects"
                  class="text-sm text-gray-600 hover:text-gray-900 transition-colors"
                >
                  Proyectos
                </router-link>
              </li>
              <li>
                <router-link
                  to="/contact"
                  class="text-sm text-gray-600 hover:text-gray-900 transition-colors"
                >
                  Contacto
                </router-link>
              </li>
            </ul>
          </div>

          <!-- Columna 3 -->
          <div>
            <h4
              class="text-sm font-semibold text-gray-900 mb-3 uppercase tracking-wider"
            >
              Conecta
            </h4>
            <div class="flex space-x-3">
              <!-- Social icons (igual que antes) -->
              <!-- ... -->
            </div>
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
};
</script>

<style>
.router-link-active {
  color: #111827 !important;
  font-weight: 500;
}
</style>
