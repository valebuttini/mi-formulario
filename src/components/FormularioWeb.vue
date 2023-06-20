<template>
    <form action="">
      <div>
        <label for="name">Mi nombre</label>
        <input type="text" id="name" v-model="name" />
        {{ name }}
      </div>
      <div>
        <label for="legal">Acepto las políticas de privacidad</label>
        <input type="checkbox" name="legal" id="legal" v-model="legal" />
      </div>
      <div>
        <h4>Selecciona tu curso</h4>
        <div>
          <input
            type="checkbox"
            id="checkJS"
            v-model="checks"
            value="javascriptdesdevalue"
          />
          <label for="checkJS">JavaScript</label>
        </div>
        <div>
          <input type="checkbox" id="checkReact" v-model="checks" value="react" />
          <label for="checkReact">React</label>
        </div>
        <div>
          <input type="checkbox" id="checkNg" v-model="checks" value="angular" />
          <label for="checkNg">Angular</label>
        </div>
        <div>
          <input type="checkbox" id="checkVue" v-model="checks" value="vue" />
          <label for="checkVue">Vue</label>
        </div>
      </div>
      <div>
        <label for="country">País</label>
        <select id="country" v-model="country">
          <option value="es">España</option>
          <option value="fr">Francia</option>
          <option value="it">Italia</option>
          <option value="pt">Portugal</option>
        </select>
        {{ country }}
      </div>
      <div>
        <label for="multiCountry">Multiple país</label>
        <select id="multiCountry" v-model="multiCountry" multiple>
          <option value="es">España</option>
          <option value="fr">Francia</option>
          <option value="it">Italia</option>
          <option value="pt">Portugal</option>
        </select>
      </div>
      <div>
        <h4>Tipo de documento</h4>
        <div>
          <input
            type="radio"
            name="documentType"
            id="documentDNI"
            v-model="document"
            value="dni"
          />
          <label for="documentDNI">DNI</label>
        </div>
        <div>
          <input
            type="radio"
            name="documentType"
            id="documentPassport"
            v-model="document"
            value="passport"
          />
          <label for="documentPassport">Pasaporte</label>
        </div>
        <div>
          <input
            type="radio"
            name="documentType"
            id="documentVisa"
            v-model="document"
            value="visa"
          />
          <label for="documentVisa">VISA</label>
        </div>
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
        country: "es",
        multiCountry: [],
        document: "",
      };
    },
  };
  </script>