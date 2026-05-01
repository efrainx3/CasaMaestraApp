<script setup lang="ts">
import AppCabecera from '../components/layout/AppCabecera.vue'
import AppFooter from '../components/layout/AppFooter.vue'
</script>

<template>
  <div class="min-h-screen flex flex-col font-sans">
    <AppCabecera />
    <main class="flex-grow">
      <slot />
    </main>
    <AppFooter />
  </div>
</template>
