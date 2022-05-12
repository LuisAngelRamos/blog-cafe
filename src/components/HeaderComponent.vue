<template>
  <header class="header">
    <div class="contenedor">
      <div class="barra">
        <router-link class="logo" to="/">
            <h1 class="logo__nombre no-margin centrar-texto">Blog<span class="logo__bold">DeCafe</span></h1>
          </router-link>
        <nav class="navegacion">
          <router-link class="navegacion__enlace" to="/about">Nosotros</router-link>
          <router-link class="navegacion__enlace" to="/cursos">Cursos</router-link>
          <router-link class="navegacion__enlace" to="/contacto">Contacto</router-link>
        </nav>
      </div>
    </div>
    <div class="header__texto centrar-texto">
      <h2 class="no-margin">Blog de cafe con Consejos y Cursos</h2>
        <p class="no-margin">Aprende de los expertos con la mejores recetas y consejos</p>
    </div>
  </header>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HeaderComponent',
  components: {
  }
}
</script>
