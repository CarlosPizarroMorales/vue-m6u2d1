<template>
  <div>
    <h1>{{ ejercicio6 }}</h1>
    <form>
      <label for="">Seleccione su animal</label>
      <select v-model="animal">
        <option value="https://images6.fanpop.com/image/photos/36800000/Beautiful-black-wolf-wolves-36825806-1600-1200.jpg">Perro</option>
        <option value="https://wallpapercave.com/wp/wp2618927.jpg">Gato</option>
        <option value="https://hdqwalls.com/wallpapers/4k-lion-hd-lo.jpg">León</option>
        <option value="https://facts.net/wp-content/uploads/2020/10/Blue-Quaker-Parrot.jpg">Loro</option>
      </select>
    </form>
    <img :src="animal" alt="">
  </div>
</template>

<script>
export default {
  name: 'FormBinding03',
  data() {
    return {
      animal: ' ',
    }
  },
  props: {
    ejercicio6: String
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

  img {
    display: block;
    width: 60vw;
    margin: 0 auto;
  }
</style>
