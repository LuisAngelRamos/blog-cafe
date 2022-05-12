<template>
  <main class="contenedor">
    <h3 class="centrar-texto">Nuestros Proximos Cursos y Talleres</h3>
    <CursoView
      title="Tecnicas de Extraccion de Cafe"
      price="Gratis"
      size="20"
      urlImage="curso1.jpg"
    />
    <CursoView
      title="Taller para Tostar y moler Granos"
      price="Gratis"
      size="20"
      urlImage="curso2.jpg"
    />
    <CursoView
      title="Recetas de Cafe para principiantes"
      price="Gratis"
      size="20"
      urlImage="curso3.jpg"
    />
  </main>
</template>

<script>
import CursoView from '@/components/CursoView.vue'
export default {
  name: 'CursosView',
  components: {
    CursoView
  }
}
</script>
