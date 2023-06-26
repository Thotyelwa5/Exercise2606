<template>
    <nav>
      <ul>
        <li>Home</li>
        <li>About</li>
        <li>Contact</li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'Navbar',
  }
  </script>
  
  <style scoped>
  nav {
    background-color: #333;
    color: #fff;
  }
  
  ul {
    list-style: none;
    display: flex;
    justify-content: space-around;
    padding: 0;
  }
  </style>
  