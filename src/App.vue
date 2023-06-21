<template>
  <div id="app">

    <FormularioValidacion />
    <ModificadoresEntrada />
    <FormularioWeb />

  </div>
</template>

<script>
import FormularioValidacion from "./components/FormularioValidacion.vue";
import ModificadoresEntrada from './components/ModificadoresEntrada.vue';
import FormularioWeb from "./components/FormularioWeb.vue";



export default {
  name: "App",
  components: {
    FormularioValidacion,
    ModificadoresEntrada,
    FormularioWeb,
  
  },
  data() {
    return {
      options: [
        { name: "Angular", value: "angular" },
        { name: "Vue", value: "vue" },
      ],
      framework: "angular",
    };
  },
};
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
