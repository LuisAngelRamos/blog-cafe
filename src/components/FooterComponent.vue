<template>
  <footer class="footer">
    <div class="contenedor">
      <div class="barra">
        <router-link class="logo" to="/">
          <h1 class="logo__nombre no-margin centrar-texto">Blog<span class="logo__bold">DeCafe</span></h1>
        </router-link>
        <nav class="navegacion">
          <router-link class="navegacion__enlace" to="/about">Nosotros</router-link>
          <router-link class="navegacion__enlace" to="/cursos">Cursos</router-link>
          <router-link class="navegacion__enlace" to="/about">Contacto</router-link>
        </nav>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComponent'
}
</script>
