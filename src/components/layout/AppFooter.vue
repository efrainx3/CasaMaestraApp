<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>

<template>
  <footer class="bg-slate-900 text-slate-300 py-12">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div>
          <h3 class="text-xl font-bold text-white mb-4">CasaMaestra</h3>
          <p class="text-sm">
            Expertos en adecuaciones locativas y construcción de obra. Transformamos tus espacios con calidad y cumplimiento.
          </p>
        </div>
        <div>
          <h4 class="text-lg font-bold text-white mb-4">Enlaces Rápidos</h4>
          <ul class="space-y-2">
            <li><RouterLink to="/" class="hover:text-white transition-colors">Inicio</RouterLink></li>
            <li><RouterLink to="/nosotros" class="hover:text-white transition-colors">Nosotros</RouterLink></li>
            <li><RouterLink to="/servicios" class="hover:text-white transition-colors">Servicios</RouterLink></li>
            <li><RouterLink to="/contactenos" class="hover:text-white transition-colors">Contáctenos</RouterLink></li>
          </ul>
        </div>
        <div>
          <h4 class="text-lg font-bold text-white mb-4">Contacto</h4>
          <address class="not-italic text-sm space-y-2">
            <p>📍 Calle Principal #123, Ciudad</p>
            <p>📞 +57 300 123 4567</p>
            <p>✉️ info@casamaestra.com</p>
          </address>
        </div>
      </div>
      <div class="mt-12 pt-8 border-t border-slate-700 text-center text-sm">
        <p>&copy; {{ new Date().getFullYear() }} CasaMaestra. Todos los derechos reservados.</p>
      </div>
    </div>
  </footer>
</template>
