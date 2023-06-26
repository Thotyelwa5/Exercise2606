<template>
    <div>
      <ul>
        <li v-for="teammate in Teammates" :key="teammate.id">
          {{ teammate.name }}
        </li>
       
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        Teammates: []
      };
    },
    mounted() {
      fetch("https://thotyelwa5.github.io/JSON-Server/index.json")
        .then((response) => response.json())
        .then((data) => {
          console.log(data);
          this.Teammates = data; 
        })
        .catch((error) => {
          console.error(error);
        });
    },
  };
  </script>
  
  <style scoped>
 
  </style>
  