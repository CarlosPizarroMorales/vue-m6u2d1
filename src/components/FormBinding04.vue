<template>
  <div>
    <h1>{{ ejercicio7 }}</h1>
    <form>
      <fieldset>
        <label for="any">¿Cómo calificarías el servicio recibido?: <span>{{ calificacion }}</span></label>
        <ul>
          <li><input type="radio" value="5" name="calificacion" v-model="calificacion" />Muy bueno</li>
          <li><input type="radio" value="4" name="calificacion" v-model="calificacion" />Bueno</li>
          <li><input type="radio" value="3" name="calificacion" v-model="calificacion" />Neutral</li>
          <li><input type="radio" value="2" name="calificacion" v-model="calificacion" />Malo</li>
          <li><input type="radio" value="1" name="calificacion" v-model="calificacion" />Muy malo</li>
        </ul>  
      </fieldset>
    </form>
  </div>
</template>

<script>
export default {
  name: 'FormBinding04',
  data() {
    return {
      calificacion: ' ',
    }
  },
  props: {
    ejercicio7: String
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

  ul {
    list-style: none;
    margin: 0;
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
