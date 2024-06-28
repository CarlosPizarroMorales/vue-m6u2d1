<template>
  <div>
    <h1>{{ ejercicio2 }}</h1>
    <p>Para más información contactarse al número: <span>{{ telefono }}</span></p>
    <input v-model="telefono" />
    <!-- <input id="nombre"> -->
  </div>
</template>

<script>
export default {
  name: 'VModel02',
  data() {
    return {
      telefono: '',
    }
  },
  props: {
    ejercicio2: String
  }
}
</script>

<style scoped>
  span {
    color: red;
  }
</style>
