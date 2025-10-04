<template>
  <div class="min-h-screen bg-white">
    <!-- Header de la página -->
    <section class="py-20 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <h1 class="text-5xl font-bold text-gray-900 mb-6">Acerca de Mí</h1>
          <p class="text-xl text-gray-600 max-w-3xl mx-auto">
            Desarrollador junior apasionado por la tecnología y el aprendizaje continuo
          </p>
        </div>
      </div>
    </section>

    <!-- Introducción personal con foto -->
    <section class="py-20 bg-white">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 items-start">
          <!-- Foto de perfil -->
          <div class="lg:col-span-1">
            <div class="sticky top-28">
              <div class="aspect-square rounded-lg overflow-hidden shadow-lg bg-gray-200">
                <img :src="profile" alt="Foto de perfil" class="w-full h-full object-cover" />
              </div>

              <!-- Información rápida -->
              <div class="mt-6 space-y-3">
                <div class="flex items-center text-gray-600">
                  <svg class="w-5 h-5 mr-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path>
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path>
                  </svg>
                  Cancún, México
                </div>
                <div class="flex items-center text-gray-600">
                  <svg class="w-5 h-5 mr-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z">
                    </path>
                  </svg>
                  albertocastrejon377@gmail.com
                </div>
                <div class="flex items-center text-gray-600">
                  <svg class="w-5 h-5 mr-3 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z">
                    </path>
                  </svg>
                  Disponible para trabajo remoto o presencial
                </div>
              </div>
            </div>
          </div>

          <!-- Contenido principal -->
          <div class="lg:col-span-2 space-y-8">
            <div>
              <h2 class="text-3xl font-bold text-gray-900 mb-6">Mi Historia</h2>
              <div class="space-y-4 text-gray-600 leading-relaxed">
                <p>
                  Desde pequeño siempre me ha interesado la tecnología y cómo las cosas
                  funcionan detrás de lo que vemos. Esa curiosidad me llevó a explorar el
                  mundo de las computadoras, el hardware y, con el tiempo, el desarrollo
                  de software. Descubrí que con unas líneas de código se pueden construir
                  soluciones reales, capaces de mejorar procesos y crear experiencias
                  únicas.
                </p>
                <p>
                  Con el paso del tiempo, he enfocado mi aprendizaje en el desarrollo web
                  y en comprender cómo se conectan las distintas partes de un sistema,
                  desde la interfaz hasta la base de datos o la red. Me gusta aprender de
                  forma autodidacta y mantenerme al día con las nuevas tecnologías.
                </p>
              </div>
            </div>

            <div>
              <h3 class="text-2xl font-bold text-gray-900 mb-4">Lo que me motiva</h3>
              <div class="space-y-4 text-gray-600 leading-relaxed">
                <p>
                  Lo que más me motiva es la posibilidad de transformar ideas en proyectos
                  funcionales. Disfruto cada etapa del proceso: desde planificar la
                  arquitectura hasta ver el resultado final en funcionamiento. También me
                  inspira el impacto que la tecnología puede tener en las personas,
                  especialmente cuando se combina un buen diseño con soluciones
                  eficientes. Para mí, cada proyecto es una oportunidad de seguir
                  aprendiendo, mejorar mis habilidades y aportar algo útil a los demás.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Educación -->
    <section class="py-20 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <h2 class="text-3xl font-bold text-gray-900 mb-12">Educación</h2>

        <div class="space-y-8">
          <!-- Item 1 -->
          <div class="bg-white rounded-lg p-8 border border-gray-200">
            <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-4">
              <div>
                <h3 class="text-xl font-semibold text-gray-900">
                  Ingeniería en Software
                </h3>
                <p class="text-gray-600 mt-1">Universidad Politécnica de Quintana Roo</p>
              </div>
              <span class="text-gray-500 mt-2 md:mt-0">2022 - 2025</span>
            </div>
            <p class="text-gray-600 leading-relaxed">
              Durante mi formación adquirí conocimientos en desarrollo de software, bases
              de datos, arquitectura de sistemas y redes (Cisco – CCNA: Introduction to
              Networks), aplicando metodologías ágiles. He participado en proyectos que
              integran frontend, backend y despliegue en servidores.
            </p>
          </div>

          <!-- Item 2 -->
          <div class="bg-white rounded-lg p-8 border border-gray-200">
            <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-4">
              <div>
                <h3 class="text-xl font-semibold text-gray-900">
                  Técnico en Sistemas y Mantenimiento de Cómputo
                </h3>
                <p class="text-gray-600 mt-1">
                  Colegio de Estudios Científicos y Tecnológicos del Estado
                </p>
              </div>
              <span class="text-gray-500 mt-2 md:mt-0">2019 - 2022</span>
            </div>
            <p class="text-gray-600 leading-relaxed">
              Formación técnica orientada al soporte de equipos de cómputo, instalación de
              redes y mantenimiento preventivo y correctivo. Incluyó fundamentos de
              programación, sistemas operativos y redes Cisco.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Experiencia / Proyectos Prácticos -->
    <section class="py-20 bg-white">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <h2 class="text-3xl font-bold text-gray-900 mb-12">Experiencia</h2>

        <div class="space-y-8">
          <!-- Item 1 -->
          <div class="border-l-4 border-gray-900 pl-8 relative">
            <div class="absolute -left-2 top-0 w-4 h-4 bg-gray-900 rounded-full"></div>
            <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-4">
              <div>
                <h3 class="text-xl font-semibold text-gray-900">
                  Plataforma de Estancias y Estadías
                </h3>
                <p class="text-gray-600 mt-1">Proyecto Académico Universitario</p>
              </div>
              <span class="text-gray-500 mt-2 md:mt-0">2025</span>
            </div>
            <p class="text-gray-600 leading-relaxed mb-4">
              Desarrollo de una plataforma web para la gestión de proyectos de estancias y
              estadías. Incluye módulos para control de usuarios, login seguro y
              administración de información académica.
            </p>
            <div class="flex flex-wrap gap-2">
              <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded">React</span>
              <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded">MySQL</span>
              <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded">UX/UI</span>
              <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded">Node.js</span>
            </div>
          </div>

          <!-- Item 2 -->
          <div class="border-l-4 border-gray-300 pl-8 relative">
            <div class="absolute -left-2 top-0 w-4 h-4 bg-gray-300 rounded-full"></div>
            <div class="flex flex-col md:flex-row md:items-start md:justify-between mb-4">
              <div>
                <h3 class="text-xl font-semibold text-gray-900">
                  Bolsa de Trabajo UPQROO
                </h3>
                <p class="text-gray-600 mt-1">Proyecto Universitario</p>
              </div>
              <span class="text-gray-500 mt-2 md:mt-0">2025</span>
            </div>
            <p class="text-gray-600 leading-relaxed mb-4">
              Desarrollo de un sistema web para conectar estudiantes con oportunidades
              laborales, incluyendo registro de empresas, publicación de vacantes y
              gestión de candidatos.
            </p>
            <div class="flex flex-wrap gap-2">
              <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded">Next.js</span>
              <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded">Express</span>
              <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded">Node.js</span>
              <span class="px-3 py-1 bg-gray-100 text-gray-700 text-sm rounded">MySQL</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Habilidades interpersonales -->
    <section class="py-20 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <h2 class="text-3xl font-bold text-gray-900 mb-12 text-center">
          Habilidades Blandas
        </h2>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
          <div class="bg-white rounded-lg p-6 border border-gray-200 text-center">
            <div class="w-12 h-12 bg-gray-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-6 h-6 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253">
                </path>
              </svg>
            </div>
            <h3 class="font-semibold text-gray-900 mb-2">Aprendizaje Rápido</h3>
            <p class="text-sm text-gray-600">
              Capacidad de adaptarme y aprender nuevas tecnologías
            </p>
          </div>

          <div class="bg-white rounded-lg p-6 border border-gray-200 text-center">
            <div class="w-12 h-12 bg-gray-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-6 h-6 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z">
                </path>
              </svg>
            </div>
            <h3 class="font-semibold text-gray-900 mb-2">Trabajo en Equipo</h3>
            <p class="text-sm text-gray-600">
              Colaboración efectiva con otros desarrolladores
            </p>
          </div>

          <div class="bg-white rounded-lg p-6 border border-gray-200 text-center">
            <div class="w-12 h-12 bg-gray-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-6 h-6 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z">
                </path>
              </svg>
            </div>
            <h3 class="font-semibold text-gray-900 mb-2">Resolución de Problemas</h3>
            <p class="text-sm text-gray-600">Enfoque analítico para superar desafíos</p>
          </div>

          <div class="bg-white rounded-lg p-6 border border-gray-200 text-center">
            <div class="w-12 h-12 bg-gray-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-6 h-6 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z">
                </path>
              </svg>
            </div>
            <h3 class="font-semibold text-gray-900 mb-2">Comunicación</h3>
            <p class="text-sm text-gray-600">Claridad al expresar ideas técnicas</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Intereses -->
    <section class="py-20 bg-white">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <h2 class="text-3xl font-bold text-gray-900 mb-6 text-center">
          Más Allá del Código
        </h2>
        <p class="text-gray-600 text-center mb-12 max-w-2xl mx-auto">
          Además del desarrollo, me gusta mantenerme activo aprendiendo, explorando nuevas
          ideas y equilibrando la parte técnica con actividades que me motivan día a día.
        </p>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <!-- NUEVO ITEM -->
          <div class="text-center">
            <div class="w-16 h-16 bg-gray-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4v16m8-8H4"></path>
              </svg>
            </div>
            <h3 class="font-semibold text-gray-900 mb-2">Tecnología y Redes</h3>
            <p class="text-sm text-gray-600">
              Me interesa aprender sobre infraestructura, redes y cómo se conectan los
              sistemas a nivel técnico.
            </p>
          </div>

          <div class="text-center">
            <div class="w-16 h-16 bg-gray-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z">
                </path>
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
              </svg>
            </div>
            <h3 class="font-semibold text-gray-900 mb-2">Tutoriales en Línea</h3>
            <p class="text-sm text-gray-600">
              Aprendizaje continuo a través de cursos y videos
            </p>
          </div>

          <div class="text-center">
            <div class="w-16 h-16 bg-gray-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10">
                </path>
              </svg>
            </div>
            <h3 class="font-semibold text-gray-900 mb-2">Proyectos Personales</h3>
            <p class="text-sm text-gray-600">Experimentación con nuevas tecnologías</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Call to action -->
    <section class="py-20 bg-gray-900">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-3xl font-bold text-white mb-4">¿Quieres saber más?</h2>
        <p class="text-gray-300 mb-8 max-w-2xl mx-auto">
          Si te interesa conocer más sobre mi trabajo o colaborar en un proyecto, no dudes
          en contactarme
        </p>
        <div class="flex flex-wrap justify-center gap-4">
          <router-link to="/projects"
            class="inline-flex items-center px-6 py-3 bg-white text-gray-900 font-medium rounded hover:bg-gray-100 transition-colors duration-200">
            Ver mis proyectos
          </router-link>
          <router-link to="/contact"
            class="inline-flex items-center px-6 py-3 border-2 border-white text-white font-medium rounded hover:bg-white hover:text-gray-900 transition-colors duration-200">
            Contactar
          </router-link>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import profile from "../assets/profile.png"

export default {
  name: "About",
  data() {
    return {
      profile
    };
  },
};
</script>

<style scoped>
/* Efecto sticky para la foto de perfil en desktop */
@media (min-width: 1024px) {
  .sticky {
    position: sticky;
  }
}
</style>
