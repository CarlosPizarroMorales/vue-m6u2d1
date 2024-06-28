<template>
  <div>
    <h1>{{ ejercicio5 }}</h1>
    <form>
      <label>Licencia clase: <span>{{ letra }}</span> </label>
      <select v-model="letra">
        <option value="A">A</option>
        <option value="B">B</option>
        <option value="C">C</option>
        <option value="D">D</option>
        <option value="E">E</option>
        <option value="F">F</option>
      </select>
    </form>
  </div>
</template>

<script>
export default {
  name: 'FormBinding02',
  data() {
    return {
      letra: ' ',
    }
  },
  props: {
    ejercicio5: String
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
</style>
