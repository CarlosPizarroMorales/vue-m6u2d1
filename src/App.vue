<template>
  <VModel01 ejercicio1="Directiva v-model: ejercicio 1"/>
  <VModel02 ejercicio2="Directiva v-model: ejercicio 2"/>
  <VBind01 ejercicio3="Directiva v-bind: ejercicio 3"/>
  <FormBinding01 ejercicio4="Directivas v-bind y v-model en formularios: ejercicio 4"/>
  <FormBinding02 ejercicio5="v-model en elemento select ejercicio 5"/>
  <FormBinding03 ejercicio6="v-model en elemento select ejercicio 6"/>
  <FormBinding04 ejercicio7="v-model en input tipo radio ejercicio 7"/>
  <FormBinding05 ejercicio8="v-model para cambiar color de un div ejercicio 8"/>
  <FormBinding06 ejercicio9="v-model en input tipo checkbox ejercicio 9"/>
</template>

<script>
import VModel01 from './components/VModel01.vue';
import VModel02 from './components/VModel02.vue';
import VBind01 from './components/VBind01.vue';
import FormBinding01 from './components/FormBinding01.vue';
import FormBinding02 from './components/FormBinding02.vue';
import FormBinding03 from './components/FormBinding03.vue';
import FormBinding04 from './components/FormBinding04.vue';
import FormBinding05 from './components/FormBinding05.vue';
import FormBinding06 from './components/FormBinding06.vue';

export default {
  name: 'App',
  components: {
    VModel01,
    VModel02,
    VBind01,
    FormBinding01,
    FormBinding02,
    FormBinding03,
    FormBinding04,
    FormBinding05,
    FormBinding06,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
