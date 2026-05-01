# Carpeta de Imágenes

En un proyecto de Vue 3 con Vite, esta es la carpeta recomendada para almacenar las imágenes de tu aplicación (como logos, banners, íconos, fondos, etc.).

## ¿Cómo usarlas en tus componentes?

Las imágenes guardadas aquí son procesadas por Vite (optimizadas y cacheadas). Para usarlas en tus archivos `.vue` (por ejemplo, en tu `Cabecera.vue`), tienes dos opciones principales:

### Opción 1: Importación directa en el script (Recomendado)

```vue
<script setup>
import logoCasaMaestra from '@/assets/images/logo.png'
</script>

<template>
  <img :src="logoCasaMaestra" alt="Logo" />
</template>
```

### Opción 2: Usar rutas relativas en el template

```vue
<template>
  <img src="../assets/images/logo.png" alt="Logo" />
  <!-- O usando el alias global @ que apunta a src/ -->
  <img src="@/assets/images/logo.png" alt="Logo" />
</template>
```

> **Nota:** Existe otra carpeta llamada `public/` en la raíz del proyecto. Esa carpeta se usa **exclusivamente** para archivos estáticos que no necesitan ser procesados por Vite, como el `favicon.ico` o el `robots.txt`. Para todo lo demás (especialmente imágenes que usarás dentro de tus vistas o componentes), usa esta carpeta `src/assets/images/`.
