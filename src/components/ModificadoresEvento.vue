<template>
    <div>
      <h2>.stop</h2>
      <div @click="handleClick">
        <button @click.stop="handleButton">
          <span @click="handleClickSpan">Stop Propagation</span>
        </button>
      </div>
      <hr />
      <h2>.capture</h2>
      <!-- un evento dirigido a un elemento hijo se maneja primero por el elemento padre -->
      <div @click.capture="handleClick">
        <button @click="handleButton">
          <span @click="handleClickSpan">Capture</span>
        </button>
      </div>
      <hr />
      <h2>.self</h2>
      <div @click="handleClick">
        <button>No self</button>
      </div>
      <div @click.self="handleClick">
        <button>Self</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "ModificadoresEvento",
    methods: {
      handleClick() {
        console.log("Abuelo: Clicked on the parent element");
      },
      handleButton() {
        console.log("Padre: Clicked on the button");
      },
      handleClickSpan() {
        console.log("Hijo: Clicked on the span");
      },
    },
  };
  </script>