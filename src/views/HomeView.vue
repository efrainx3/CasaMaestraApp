<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>

<template>
  <div class="flex flex-col">
    <!-- Hero Section -->
    <section class="relative bg-slate-900 text-white overflow-hidden">
      <!-- Decorative background -->
      <div class="absolute inset-0 z-0 opacity-40">
        <div class="absolute inset-0 bg-gradient-to-r from-slate-900 via-slate-900/80 to-transparent z-10"></div>
        <!-- Placeholder pattern that looks like an architectural grid -->
        <div class="h-full w-full opacity-30" style="background-image: radial-gradient(#3b82f6 1px, transparent 1px); background-size: 30px 30px;"></div>
      </div>
      
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-24 md:py-32 relative z-10">
        <div class="max-w-3xl">
          <span class="inline-block py-1 px-3 rounded-full bg-blue-900/50 border border-blue-700/50 text-blue-300 text-sm font-semibold mb-6 tracking-wide">
            Excelencia en Construcción
          </span>
          <h1 class="text-5xl md:text-6xl font-extrabold tracking-tight mb-6 leading-tight">
            Transformamos tus espacios en <span class="text-secondary">obras maestras</span>
          </h1>
          <p class="text-xl text-slate-300 mb-10 max-w-2xl leading-relaxed">
            Especialistas en adecuaciones locativas, remodelaciones y construcción de obra civil. Calidad, cumplimiento y diseño de vanguardia para tu proyecto.
          </p>
          <div class="flex flex-col sm:flex-row gap-4">
            <RouterLink to="/contactenos" class="bg-secondary hover:bg-amber-600 text-slate-900 font-bold py-4 px-8 rounded-lg text-center transition-all duration-300 transform hover:-translate-y-1 shadow-lg hover:shadow-amber-500/30">
              Solicitar Presupuesto
            </RouterLink>
            <RouterLink to="/servicios" class="bg-white/10 hover:bg-white/20 border border-white/20 text-white font-medium py-4 px-8 rounded-lg text-center transition-all duration-300 backdrop-blur-sm">
              Conoce Nuestros Servicios
            </RouterLink>
          </div>
        </div>
      </div>
    </section>

    <!-- Features / Value Proposition Section -->
    <section class="py-20 bg-slate-50">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-16">
          <h2 class="text-primary font-semibold tracking-wide uppercase text-sm mb-2">Por qué elegirnos</h2>
          <h3 class="text-3xl md:text-4xl font-bold text-slate-900 mb-4">Construimos con propósito</h3>
          <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <!-- Feature 1 -->
          <div class="bg-white rounded-2xl p-8 shadow-sm hover:shadow-xl transition-shadow duration-300 border border-slate-100 group">
            <div class="w-14 h-14 bg-blue-50 text-primary rounded-xl flex items-center justify-center mb-6 group-hover:bg-primary group-hover:text-white transition-colors duration-300">
              <svg xmlns="http://www.w3.org/0000.svg" class="h-7 w-7" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4" />
              </svg>
            </div>
            <h4 class="text-xl font-bold text-slate-900 mb-3">Obra Civil</h4>
            <p class="text-slate-600 leading-relaxed">
              Diseño y ejecución de proyectos de construcción desde cero, cumpliendo con los más altos estándares técnicos y normativos.
            </p>
          </div>

          <!-- Feature 2 -->
          <div class="bg-white rounded-2xl p-8 shadow-sm hover:shadow-xl transition-shadow duration-300 border border-slate-100 group">
            <div class="w-14 h-14 bg-amber-50 text-secondary rounded-xl flex items-center justify-center mb-6 group-hover:bg-secondary group-hover:text-white transition-colors duration-300">
              <svg xmlns="http://www.w3.org/0000.svg" class="h-7 w-7" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 10l-2 1m0 0l-2-1m2 1v2.5M20 7l-2 1m2-1l-2-1m2 1v2.5M14 4l-2-1-2 1M4 7l2-1M4 7l2 1M4 7v2.5M12 21l-2-1m2 1l2-1m-2 1v-2.5M6 18l-2-1v-2.5M18 18l2-1v-2.5" />
              </svg>
            </div>
            <h4 class="text-xl font-bold text-slate-900 mb-3">Adecuaciones Locativas</h4>
            <p class="text-slate-600 leading-relaxed">
              Remodelación y optimización de espacios residenciales y comerciales para mejorar su funcionalidad y estética.
            </p>
          </div>

          <!-- Feature 3 -->
          <div class="bg-white rounded-2xl p-8 shadow-sm hover:shadow-xl transition-shadow duration-300 border border-slate-100 group">
            <div class="w-14 h-14 bg-blue-50 text-primary rounded-xl flex items-center justify-center mb-6 group-hover:bg-primary group-hover:text-white transition-colors duration-300">
              <svg xmlns="http://www.w3.org/0000.svg" class="h-7 w-7" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" />
              </svg>
            </div>
            <h4 class="text-xl font-bold text-slate-900 mb-3">Calidad Garantizada</h4>
            <p class="text-slate-600 leading-relaxed">
              Utilizamos materiales de primera y mano de obra experta para asegurar la durabilidad y excelencia de cada proyecto.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Call to Action -->
    <section class="bg-primary py-16">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-3xl font-bold text-white mb-6">¿Listo para iniciar tu próximo proyecto?</h2>
        <p class="text-blue-100 mb-8 max-w-2xl mx-auto text-lg">
          Nuestro equipo de expertos está preparado para asesorarte y hacer realidad tu visión con el más alto nivel de profesionalismo.
        </p>
        <RouterLink to="/contactenos" class="inline-block bg-white text-primary font-bold py-4 px-10 rounded-lg transition-transform hover:scale-105 shadow-xl">
          Contáctanos Hoy Mismo
        </RouterLink>
      </div>
    </section>
  </div>
</template>
