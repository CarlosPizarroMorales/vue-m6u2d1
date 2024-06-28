<template>
  <div>
    <h1>{{ ejercicio4 }}</h1>
    <form>
      <fieldset>
        <label for="any">{{ mensaje }}</label>
        <input v-model="mensaje" type="text" name="any">
      </fieldset>
    </form>
  </div>
</template>

<script>
export default {
  name: 'FormBinding01',
  data() {
    return {
      mensaje: ' ',
    }
  },
  props: {
    ejercicio4: String
  }
}
</script>

<style scoped>
  form {
    background: #00000033;
    width: clamp(200px, 30vw, 400px);
    margin: 1rem auto;
    text-align: center;
  }
  input, label {
    display: block;
  }
</style>
