<template>
  <div id="app">

    <FormularioValidacion />
    <ModificadoresEntrada />
    <FormularioWeb />
    <SelectDinamico :options="options" label="Select dinámico" id="dynamic" v-model="framework" />

  </div>
</template>

<script>
import FormularioValidacion from "./components/FormularioValidacion.vue";
import ModificadoresEntrada from './components/ModificadoresEntrada.vue';
import FormularioWeb from "./components/FormularioWeb.vue";
import SelectDinamico from "./components/SelectDinamico.vue";


export default {
  name: "App",
  components: {
    FormularioValidacion,
    ModificadoresEntrada,
    FormularioWeb,
    SelectDinamico,
  
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
