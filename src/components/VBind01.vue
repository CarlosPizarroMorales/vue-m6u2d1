<template>
  <div>
    <h1>{{ ejercicio3 }}</h1>
    <p>Estas imágenes están obteniendo el valor de su atributo src de forma dinámica desde el objeto data</p>
    <!-- Sintaxis de la directiva -->
    <img v-bind:src="perritoSrc" alt="un perrito">
    <!-- Sintaxis abreviada de la directiva -->
    <img :src="perritoSrc" alt="un perrito">
    <!-- <input id="nombre"> -->
  </div>
</template>

<script>
export default {
  name: 'VBind01',
  data() {
    return {
      perritoSrc: "https://i.imgur.com/Y0QQmIK.jpeg",
    };
  },
  props: {
    ejercicio3: String
  }
}
</script>

<style scoped>
  img {
    width: clamp(200px, 20vw, 400px);
    display: block;
    margin: 1rem auto;
  }
</style>
