<template>
  <div>
    <h1>{{ ejercicio9 }}</h1>
    <form>
      <label>Lenguajes de programación que domina: </label>
      <ul>
        <li><input v-model="lenguajes" name="lenguajes" type="checkbox" value="html" />HTML</li>
        <li><input v-model="lenguajes" name="lenguajes" type="checkbox" value="css" />CSS</li>
        <li><input v-model="lenguajes" name="lenguajes" type="checkbox" value="python" />Python</li>
        <li><input v-model="lenguajes" name="lenguajes" type="checkbox" value="javascript" />Javascript</li>
        <li><input v-model="lenguajes" name="lenguajes" type="checkbox" value="go" />Go</li>
        <li><input v-model="lenguajes" name="lenguajes" type="checkbox" value="php" />PHP</li>
      </ul>
    </form>
    {{ lenguajes }}
  </div>
</template>

<script>
export default {
  name: 'FormBinding06',
  data() {
    return {
      lenguajes: [],
    }
  },
  props: {
    ejercicio9: String
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

  li {
    display: flex;
    align-items: center;
  }

  span {
    font-size: 1.5rem;
    font-weight: bold;
  }
</style>
