<template>
  <div>
    <h1>{{ ejercicio8 }}</h1>
    <form>
      <label>Elige color: <span>{{ color }}</span></label>
      <select v-model="color">
        <option value="blue">Azul</option>
        <option value="red">Rojo</option>
        <option value="black">Negro</option>
      </select>
    </form>
    <div class="caja" :style="{ backgroundColor: color }"></div>
  </div>
</template>

<script>
export default {
  name: 'FormBinding05',
  data() {
    return {
      color: "yellow",
    }
  },
  props: {
    ejercicio8: String
  }
}
</script>

<style scoped>
  form {
    background: rgb(253, 226, 231);
    width: clamp(200px, 30vw, 400px);
    margin: 1rem auto;
    padding: 1rem;
    text-align: left;
  }
  input, select {
    display: block;
    margin-top: 0.5rem;
  }

  span {
    font-size: 1.5rem;
    font-weight: bold;
  }

  .caja {
    width: 300px;
    aspect-ratio: 1;
    margin: 1rem auto;
  }
</style>
