<template>
  <article class="entrada">
    <div class="entrada__imagen">
      <img loading="lazy" :src="resolve_img_url(urlImage)" alt="imagen blog">
    </div>

    <div class="entrada__contenido">
      <h4 class="no-margin">{{title}}</h4>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.
        Quae accusamus eos minima rem dolore. Architecto exercitationem beatae
        voluptate at quisquam adipisci, quas harum quidem. Fugit molestiae beatae
        ratione quod sed!</p>
        <router-link class="boton boton--primario" to="/entrada">Leer Entrada</router-link>
    </div>
  </article>
</template>

<script>
export default {
  name: 'EntradaComponent',
  props: {
    title: String,
    urlImage: String
  },
  methods: {
    resolve_img_url (path) {
      const images = require.context('../../public/assets/img/', false, /\.png$|\.jpg$/)
      return images(`./${path}`)
    }
  }
}
</script>
