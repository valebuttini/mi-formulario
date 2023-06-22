<template>
    <ul>
        <li v-for=" producto in articulos" :key="producto.id">
            {{ producto.titulo }} - {{ producto.informacion }} - {{ producto.precio }} <button>Agregar al carrito</button> 
        </li>
        
    </ul>
 </template>
      
      <script>
      const articulos = [
        {
            titulo: "Carne a las brasas",
            precio: 200, 
            informacion: "Especial blend 2 horas de coccion",
            id: 1,

        },
        {
            titulo: "Empanadas",
            precio: 50,
            informacion: "Tradicionales cortadas a cuchillo",
            id:2,
        },
        {
            titulo: "Cordero patagonico",
            precio: 400,
            informacion: "Especial cordero de la patagonia",
            id: 3,

        },
        {
            titulo: "Locro",
            precio: 500,
            informacion: "Locro tradicional con fritura",
            id: 4,

        },
      ];
      export default {
        name: "ListaProductos",
        data() {
          return {
            articulos
          }
        }
      }
      </script>
