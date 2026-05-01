<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>

<template>
  <header class="bg-white shadow-sm sticky top-0 z-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center h-20">
        <!-- Logo en el costado izquierdo -->
        <div class="flex-shrink-0 flex items-center">
          <RouterLink to="/" class="flex items-center gap-2 group">
            <div class="w-40 h-80 flex items-center justify-center text-white font-bold text-xl transition-transform group-hover:scale-105">
              <img src="@/assets/images/Logo_Nombre_Rectangular.png" alt="Logo CasaMaestra">
            </div>
          </RouterLink>
        </div>

        <!-- Opciones desde la mitad hacia la derecha -->
        <nav class="hidden md:flex flex-1 justify-end items-center space-x-8">
          <RouterLink to="/nosotros" class="text-slate-600 hover:text-primary font-medium transition-colors duration-200">
            Nosotros
          </RouterLink>
          <RouterLink to="/servicios" class="text-slate-600 hover:text-primary font-medium transition-colors duration-200">
            Servicios
          </RouterLink>
          <RouterLink to="/contactenos" class="text-slate-600 hover:text-primary font-medium transition-colors duration-200">
            Contáctenos
          </RouterLink>

          <RouterLink to="/contactenos" class="bg-primary hover:bg-blue-800 text-white px-5 py-2.5 rounded-md font-medium transition-colors duration-200 shadow-sm">
            Cotizar Proyecto
          </RouterLink>
        </nav>

        <!-- Botón menú móvil (opcional/básico) -->
        <div class="md:hidden flex items-center">
          <button class="text-slate-600 hover:text-primary">
            <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
          </button>
        </div>
      </div>
    </div>
  </header>
</template>
