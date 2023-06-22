<template>
<div>
    <div>
        <label for="tittle">BIENVENIDOS A OSTERIA V-BIN </label>
    </div>
    <div>
        <label for="subtittle">Registrate para una mejor experiencia</label>
    </div>
</div>
  </template>
  
  <script>
  export default {
    name: "ComponenteInicio",
    data() {
      return {
        tittle: "string",
        subtittle: "string",
      };
    },
  };
  </script>
  <style>
  #card{
    background-color: #2c3e50;

  }
  </style>