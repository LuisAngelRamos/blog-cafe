<template>
  <div class="contenedor">
    <h3 class="centrar-texto">Contacto</h3>
    <div class="contacto--bg"></div>
    <form class="formulario">
      <div class="campo">
        <label class="campo__label" for="nombre">Nombre:</label>
        <input
          class="campo__field"
          type="text"
          id="nombre"
          placeholder="Tu Nombre"
        />
      </div>
      <div class="campo">
        <label class="campo__label" for="email">Email:</label>
        <input
          class="campo__field"
          type="email"
          id="email"
          placeholder="Tu Email"
        />
      </div>
      <div class="campo">
        <label class="campo__label" for="mensaje">Mensaje:</label>
        <textarea
          id="mensaje"
          class="campo__field campo__field--textarea"
        ></textarea>
      </div>
      <div class="campo">
        <input
          type="submit"
          value="Enviar"
          class="boton boton--primario"
        />
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: 'ContactoView'
}
</script>
