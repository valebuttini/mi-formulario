<template>
    <div>
      <div>
        <label for="age">Edad</label>
        <input type="number" v-model.number="age" id="age" />
      </div>
      <div>
        <label for="email">Email</label>
        <input type="email" id="email" />
      </div>
      <div>
        <label for="address">Direccion</label>
        <input type="address" id="address" />
      </div>
      <button>Log in</button>
    </div>
  </template>
  
  <script>
  export default {
    name: "ModificadoresEntrada",
    data() {
      return {
        age: 0,
        email: "",
        address:"",
      };
    },
  };
  </script>