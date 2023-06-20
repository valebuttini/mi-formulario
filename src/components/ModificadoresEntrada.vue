<template>
    <div>
      <div>
        <label for="age"></label>
        <input type="number" v-model.number="age" id="age" />
      </div>
      <div>
        <label for="text">Text trim</label>
        <input type="text" v-model.trim="text" id="text" />
      </div>
      <div>
        <label for="lazytext">Text lazy</label>
        <!-- actualiza en el change, no en el input -->
        <input type="text" v-model.lazy="lazyText" id="lazytext" />
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "ModificadoresEntrada",
    data() {
      return {
        age: 0,
        text: "",
        lazyText: "",
      };
    },
  };
  </script>