<template>
  <div class="contenedor contenido-principal">
    <main class="blog">
      <h3>Nuestro Blog</h3>
      <EntradaComponent title='Tipos de Grano de Cafe' urlImage='blog1.jpg' />
      <EntradaComponent title='Deliciosas recetas de Cafe' urlImage='blog2.jpg' />
      <EntradaComponent title='Beneficios del Cafe' urlImage='blog3.jpg' />
    </main>
    <aside class="sidebar">
      <h3>Nustros Cursos y Talleres</h3>
      <ul class="cursos no-padding">
        <CursoSidebar title="Tecnicas de Extraccion de cafe" price="Gratis" size="20" />
        <CursoSidebar title="Recetas de Cafe para Principiantes" price="Gratis" size="20" />
      </ul>
    </aside>
  </div>
</template>

<script>
import EntradaComponent from '@/components/EntradaComponent.vue'
import CursoSidebar from '@/components/CursoSidebar.vue'
export default {
  name: 'HomeView',
  components: {
    EntradaComponent,
    CursoSidebar
  }
}
</script>
