<template>
    <div>
      <div>
        <label for="age">Edad</label>
        <input type="number" v-model.number="age" id="age" />
      </div>

    </div>
  </template>
  
  <script>
  export default {
    name: "ModificadoresEntrada",
    data() {
      return {
        age: 0,
      };
    },
  };
  </script>