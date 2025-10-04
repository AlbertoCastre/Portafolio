<template>
  <div class="min-h-screen bg-white">
    <!-- Header de la página -->
    <section class="py-20 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <h1 class="text-5xl font-bold text-gray-900 mb-6">Contacto</h1>
          <p class="text-xl text-gray-600 max-w-3xl mx-auto">
            ¿Tienes un proyecto en mente o quieres colaborar? Me encantaría escucharte
          </p>
        </div>
      </div>
    </section>
    
    <!-- Contenido principal -->
    <section class="py-20 bg-white">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
          <!-- Información de contacto -->
          <div>
            <h2 class="text-3xl font-bold text-gray-900 mb-6">Información de Contacto</h2>
            <p class="text-gray-600 mb-8 leading-relaxed">
              Estoy disponible para oportunidades de trabajo freelance, colaboraciones en proyectos interesantes y
              desarrollo web.
            </p>
            
            <!-- Tarjetas de contacto -->
            <div class="space-y-4 mb-12">
              <!-- Email -->
              <a href="mailto:albertocastrejon377@gmail.com?subject=Contacto%20desde%20la%20web&body=Hola%2C%20quiero%20hablar%20sobre%20un%20proyecto..."
                class="flex items-start p-6 bg-gray-50 rounded-lg border border-gray-200 hover:border-indigo-600 hover:shadow-md transition-all duration-200 group">
                <div
                  class="w-12 h-12 bg-white rounded-lg flex items-center justify-center mr-4 group-hover:bg-indigo-600 transition-colors duration-200 flex-shrink-0">
                  <svg class="w-6 h-6 text-gray-700 group-hover:text-white transition-colors duration-200" fill="none"
                    stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z">
                    </path>
                  </svg>
                </div>
                <div>
                  <h3 class="font-semibold text-gray-900 mb-1">Email</h3>
                  <p class="text-gray-600 break-all">albertocastrejon377@gmail.com</p>
                </div>
              </a>
              
              <!-- LinkedIn -->
              <a href="https://linkedin.com/in/alberto-castrejon-4609982b7" target="_blank" rel="noopener noreferrer"
                class="flex items-start p-6 bg-gray-50 rounded-lg border border-gray-200 hover:border-blue-600 hover:shadow-md transition-all duration-200 group">
                <div
                  class="w-12 h-12 bg-white rounded-lg flex items-center justify-center mr-4 group-hover:bg-blue-600 transition-colors duration-200 flex-shrink-0">
                  <svg class="w-6 h-6 text-gray-700 group-hover:text-white transition-colors duration-200"
                    fill="currentColor" viewBox="0 0 24 24">
                    <path
                      d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z" />
                  </svg>
                </div>
                <div>
                  <h3 class="font-semibold text-gray-900 mb-1">LinkedIn</h3>
                  <p class="text-gray-600">linkedin.com/in/alberto-castrejon</p>
                </div>
              </a>
              
              <!-- GitHub -->
              <a href="https://github.com/AlbertoCastre" target="_blank" rel="noopener noreferrer"
                class="flex items-start p-6 bg-gray-50 rounded-lg border border-gray-200 hover:border-gray-900 hover:shadow-md transition-all duration-200 group">
                <div
                  class="w-12 h-12 bg-white rounded-lg flex items-center justify-center mr-4 group-hover:bg-gray-900 transition-colors duration-200 flex-shrink-0">
                  <svg class="w-6 h-6 text-gray-700 group-hover:text-white transition-colors duration-200"
                    fill="currentColor" viewBox="0 0 24 24">
                    <path
                      d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z" />
                  </svg>
                </div>
                <div>
                  <h3 class="font-semibold text-gray-900 mb-1">GitHub</h3>
                  <p class="text-gray-600">github.com/AlbertoCastre</p>
                </div>
              </a>
            </div>
          </div>
          
          <!-- Formulario de contacto -->
          <div>
            <h2 class="text-3xl font-bold text-gray-900 mb-6">Envía un Mensaje</h2>
            <form @submit.prevent="handleSubmit" class="space-y-6">
              <!-- Nombre -->
              <div>
                <label for="name" class="block text-sm font-medium text-gray-900 mb-2">
                  Nombre completo
                </label>
                <input 
                  type="text" 
                  id="name" 
                  v-model="form.name" 
                  required
                  @blur="validateField('name')"
                  :class="{'border-red-500 focus:ring-red-500': errors.name}"
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-600 focus:border-transparent transition-all duration-200"
                  placeholder="Tu nombre" />
                <p v-if="errors.name" class="mt-1 text-sm text-red-600">{{ errors.name }}</p>
              </div>
              
              <!-- Email -->
              <div>
                <label for="email" class="block text-sm font-medium text-gray-900 mb-2">
                  Email
                </label>
                <input 
                  type="email" 
                  id="email" 
                  v-model="form.email" 
                  required
                  @blur="validateField('email')"
                  :class="{'border-red-500 focus:ring-red-500': errors.email}"
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-600 focus:border-transparent transition-all duration-200"
                  placeholder="tu@email.com" />
                <p v-if="errors.email" class="mt-1 text-sm text-red-600">{{ errors.email }}</p>
              </div>
              
              <!-- Asunto -->
              <div>
                <label for="subject" class="block text-sm font-medium text-gray-900 mb-2">
                  Asunto
                </label>
                <input 
                  type="text" 
                  id="subject" 
                  v-model="form.subject" 
                  required
                  @blur="validateField('subject')"
                  :class="{'border-red-500 focus:ring-red-500': errors.subject}"
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-600 focus:border-transparent transition-all duration-200"
                  placeholder="¿En qué puedo ayudarte?" />
                <p v-if="errors.subject" class="mt-1 text-sm text-red-600">{{ errors.subject }}</p>
              </div>
              
              <!-- Mensaje -->
              <div>
                <label for="message" class="block text-sm font-medium text-gray-900 mb-2">
                  Mensaje
                </label>
                <textarea 
                  id="message" 
                  v-model="form.message" 
                  required 
                  rows="6"
                  @blur="validateField('message')"
                  :class="{'border-red-500 focus:ring-red-500': errors.message}"
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-indigo-600 focus:border-transparent transition-all duration-200 resize-none"
                  placeholder="Cuéntame sobre tu proyecto..."></textarea>
                <p v-if="errors.message" class="mt-1 text-sm text-red-600">{{ errors.message }}</p>
              </div>
              
              <!-- Botón de envío -->
              <button 
                type="submit"
                :disabled="loading || !isFormValid"
                :class="{'opacity-50 cursor-not-allowed': loading || !isFormValid}"
                class="w-full px-6 py-4 bg-gray-900 text-white font-medium rounded-lg hover:bg-gray-800 transition-colors duration-200 flex items-center justify-center">
                <svg v-if="loading" class="animate-spin -ml-1 mr-3 h-5 w-5 text-white" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
                  <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                  <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
                </svg>
                <span v-if="loading">Enviando...</span>
                <span v-else>Enviar Mensaje</span>
                <svg v-if="!loading" class="w-5 h-5 ml-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path>
                </svg>
              </button>
            </form>
            
            <!-- Mensaje de éxito o error -->
            <transition name="fade">
              <div v-if="statusMessage" class="mt-6 p-4 rounded-lg flex items-start"
                   :class="messageType === 'success' ? 'bg-green-50 border border-green-200' : 'bg-red-50 border border-red-200'">
                <svg v-if="messageType === 'success'" class="w-5 h-5 text-green-600 mt-0.5 mr-3 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                </svg>
                <svg v-else class="w-5 h-5 text-red-600 mt-0.5 mr-3 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z" clip-rule="evenodd"/>
                </svg>
                <div>
                  <p class="text-sm font-medium" :class="messageType === 'success' ? 'text-green-800' : 'text-red-800'">
                    {{ statusMessage }}
                  </p>
                </div>
              </div>
            </transition>
          </div>
        </div>
      </div>
    </section>
    
    <!-- Sección adicional -->
    <section class="py-20 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <h2 class="text-3xl font-bold text-gray-900 mb-6">Otras formas de conectar</h2>
          <p class="text-gray-600 mb-12 max-w-2xl mx-auto">
            También puedes encontrarme en estas plataformas
          </p>
          <div class="flex justify-center space-x-6">
            <!-- LinkedIn -->
            <a href="https://linkedin.com/in/alberto-castrejon-4609982b7" target="_blank" rel="noopener noreferrer"
              class="w-14 h-14 bg-white border-2 border-gray-200 rounded-lg flex items-center justify-center hover:border-blue-600 hover:bg-blue-600 group transition-all duration-200"
              aria-label="LinkedIn">
              <svg class="w-6 h-6 text-gray-700 group-hover:text-white transition-colors duration-200"
                fill="currentColor" viewBox="0 0 24 24">
                <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z" />
              </svg>
            </a>
            
            <!-- GitHub -->
            <a href="https://github.com/AlbertoCastre" target="_blank" rel="noopener noreferrer"
              class="w-14 h-14 bg-white border-2 border-gray-200 rounded-lg flex items-center justify-center hover:border-gray-900 hover:bg-gray-900 group transition-all duration-200"
              aria-label="GitHub">
              <svg class="w-6 h-6 text-gray-700 group-hover:text-white transition-colors duration-200"
                fill="currentColor" viewBox="0 0 24 24">
                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z" />
              </svg>
            </a>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import emailjs from "@emailjs/browser";

export default {
  name: 'Contact',
  data() {
    return {
      form: {
        name: '',
        email: '',
        subject: '',
        message: ''
      },
      errors: {
        name: '',
        email: '',
        subject: '',
        message: ''
      },
      loading: false,
      statusMessage: '',
      messageType: 'success'
    }
  },
  computed: {
    isFormValid() {
      return this.form.name.trim().length >= 2 &&
             this.isValidEmail(this.form.email) &&
             this.form.subject.trim().length >= 3 &&
             this.form.message.trim().length >= 10 &&
             !Object.values(this.errors).some(error => error);
    }
  },
  methods: {
    isValidEmail(email) {
      const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      return emailRegex.test(email);
    },
    
    validateField(fieldName) {
      this.errors[fieldName] = '';
      
      switch(fieldName) {
        case 'name':
          if (this.form.name.trim().length < 2) {
            this.errors.name = 'El nombre debe tener al menos 2 caracteres';
          } else if (this.form.name.trim().length > 50) {
            this.errors.name = 'El nombre es demasiado largo';
          }
          break;
          
        case 'email':
          if (!this.form.email.trim()) {
            this.errors.email = 'El email es requerido';
          } else if (!this.isValidEmail(this.form.email)) {
            this.errors.email = 'Por favor ingresa un email válido';
          }
          break;
          
        case 'subject':
          if (this.form.subject.trim().length < 3) {
            this.errors.subject = 'El asunto debe tener al menos 3 caracteres';
          } else if (this.form.subject.trim().length > 100) {
            this.errors.subject = 'El asunto es demasiado largo';
          }
          break;
          
        case 'message':
          if (this.form.message.trim().length < 10) {
            this.errors.message = 'El mensaje debe tener al menos 10 caracteres';
          } else if (this.form.message.trim().length > 1000) {
            this.errors.message = 'El mensaje es demasiado largo';
          }
          break;
      }
    },
    
    validateAllFields() {
      this.validateField('name');
      this.validateField('email');
      this.validateField('subject');
      this.validateField('message');
      
      return !Object.values(this.errors).some(error => error);
    },
    
    async handleSubmit() {
      if (!this.validateAllFields()) {
        this.messageType = 'error';
        this.statusMessage = 'Por favor corrige los errores en el formulario';
        return;
      }
      
      this.loading = true;
      this.statusMessage = '';
      
      try {
        await emailjs.send(
          'service_x28c5ek',      
          'template_jf14acl',     
          {
            name: this.form.name,
            email: this.form.email,
            subject: this.form.subject,
            message: this.form.message
          },
          'ZfPJV-goAMRdR9ULb'       
        );
        
        this.messageType = 'success';
        this.statusMessage = '¡Mensaje enviado con éxito! Te responderé lo antes posible.';
        
        this.form = {
          name: '',
          email: '',
          subject: '',
          message: ''
        };
        
        this.errors = {
          name: '',
          email: '',
          subject: '',
          message: ''
        };
        
        setTimeout(() => {
          this.statusMessage = '';
        }, 8000);
        
      } catch (error) {
        console.error('Error al enviar el correo:', error);
        this.messageType = 'error';
        this.statusMessage = 'Ocurrió un error al enviar el mensaje. Por favor intenta nuevamente o contáctame directamente por email.';
      } finally {
        this.loading = false;
      }
    }
  }
}
</script>

<style scoped>
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.3s ease;
}
.fade-enter-from, .fade-leave-to {
  opacity: 0;
}
</style>