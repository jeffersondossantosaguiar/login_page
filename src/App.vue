<template>
  <div id="app">
    <Login />
  </div>
</template>

<script>
import Login from './components/Login'

export default {
  components: {
    Login
  }
}
</script>

<style>
@font-face {
  font-family: "Mukta";
  src: url("./fonts/Mukta-SemiBold.ttf");
}

* {
  font-family: "Mukta";
}

body {
  margin: 0;
  color: #fff;
  background-image: linear-gradient(to right bottom, #051937, #004d7a, #008793, #00bf72, #a8eb12);
}

#app {
  display: flex; /* A propriedade CSS  display especifica o tipo de caixa de renderização usada por um elemento */
  flex-direction: column;
  height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
