<template>
  <div id="app">
    <ComponenteInicio />
    <ListaProductos />
    <FormularioValidacion />
    <ModificadoresEntrada />
    <FormularioWeb />
  </div>
</template>

<script>
import ComponenteInicio from "./components/ComponenteInicio.vue";
import ListaProductos from "./components/ListaProductos.vue";
import FormularioValidacion from "./components/FormularioValidacion.vue";
import ModificadoresEntrada from './components/ModificadoresEntrada.vue';
import FormularioWeb from "./components/FormularioWeb.vue";




export default {
  name: "App",
  components: {
    ComponenteInicio,
    ListaProductos,
    FormularioValidacion,
    ModificadoresEntrada,
    FormularioWeb,
  },
  data() {
    return {

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
  background-color: rgb(201, 201, 201);
  margin-top: 60px;
}
</style>
