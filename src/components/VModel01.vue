<template>
  <div>
    <h1>{{ ejercicio1 }}</h1>
    <p>Bievenidos al curso de <span>{{ nombreDelCurso }}</span></p>
    <input v-model="nombreDelCurso" />
    <!-- <input id="nombre"> -->
  </div>
</template>

<script>
export default {
  name: 'VModel01',
  data() {
    return {
      nombreDelCurso: '',
    }
  },
  props: {
    ejercicio1: String
  }
}
</script>

<style scoped>
  span {
    color: green;
  }
</style>
