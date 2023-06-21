<template>
    <form @submit.prevent="submitHandler">
      <label for="name">Nombre completo</label>
      <input type="text" id="name" v-model="name" />
      <button>Enviar</button>
    </form> 
  </template>
  
  <script>
  export default {
      name: "FormularioValidacion",
      data() {
          return {
              name: "",

          };
      },
      methods: {
          submitHandler() {
              if (this.name === "") {
                  alert("El nombre es obligatorio");
                  return;
              }
              alert("Formulario enviado");
          },
      },
  }
  </script>