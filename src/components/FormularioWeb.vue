<template>
    <form action="">
      <div>
      </div>

      <div>
        <h4>Selecciona tu experiencia </h4>
        <div>
          <input
            type="checkbox"
            id="checkJS"
            v-model="checks"
            value="javascriptdesdevalue"
          />
          <label for="checkJS">Excelente</label>
        </div>
        <div>
          <input type="checkbox" id="checkBuena" v-model="checks" value="buena" />
          <label for="checkBuena">Buena</label>
        </div>
        <div>
          <input type="checkbox" id="checkRegular" v-model="checks" value="regular" />
          <label for="checkRegular">Regular</label>
        </div>
        <div>
          <input type="checkbox" id="checkMala" v-model="checks" value="mala" />
          <label for="checkMala">Mala</label>
        </div>
      </div>
      <div>
        <h4>Calidad de la atencion del 1-3</h4>
        <div>
          <input
            type="radio"
            name="numberOne"
            id="numberOne"
            v-model="puntuacion"
            value="one"
          />
          <label for="numberOne">1</label>
        </div>
        <div>
          <input
            type="radio"
            name="numbertwo"
            id="numbertwo"
            v-model="puntuacion"
            value="two"
          />
          <label for="numbertwo">2</label>
        </div>
        <div>
          <input
            type="radio"
            name="numberthree"
            id="numberthree"
            v-model="puntuacion"
            value="three"
          />
          <label for="numberthree">3</label>
        </div>
      </div>
      <div>
        <label for="legal">Acepto las políticas de privacidad</label>
        <input type="checkbox" name="legal" id="legal" v-model="legal" />
      </div>
      <button>Enviar</button>
    </form>
  </template>
  
  <script>
  export default {
    name: "FormularioWeb",
    data() {
      return {
        name: "",
        legal: false,
        checks: [],
        puntuacion: "",
      };
    },
  };
  </script>