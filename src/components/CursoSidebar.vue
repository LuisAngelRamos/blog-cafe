<template>
  <li class="widget-curso">
    <h4 class="no-margin">{{title}}</h4>
    <p class="widget-curso__label">Precio:
      <span class="widget-curso__info">{{price}}</span>
    </p>
    <p class="widget-curso__label">Cupo:
      <span class="widget-curso__info">{{size}}</span>
    </p>
    <router-link class="boton boton--secundario" to="/">Mas Informacion</router-link>
  </li>
</template>

<script>
export default {
  name: 'CursoSidebar',
  props: {
    price: String,
    size: Number,
    title: String
  }
}
</script>
