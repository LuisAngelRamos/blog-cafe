<template>
  <div class="curso">
    <div class="curso__imagen">
      <img :src="resolve_img_url(urlImage)" alt="Imagen curso">
    </div>
    <div class="curso__informacion">
      <h4 class="no-margin">{{title}}</h4>
      <p class="curso__label">Precio:
        <span class="curso__info">{{price}}</span>
      </p>
      <p class="curso__label">Cupo:
        <span class="curso__info">{{size}}</span>
      </p>
      <p class="curso__descripcion">Lorem ipsum dolor sit amet,
        consectetur adipisicing elit. Dolorum dolor libero
        pariatur ipsam nulla id molestiae minus ipsum nemo labore,
        a facilis doloremque itaque,
        cupiditate numquam error eius dicta hic!
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CursoView',
  props: {
    title: String,
    price: String,
    size: String,
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
