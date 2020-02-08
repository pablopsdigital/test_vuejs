<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Mi nueva aplicación en Vue.js App"/>
    <MiComponente></MiComponente>
    <MiBoton textoBoton='Login' color='orange'></MiBoton>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MiComponente from './components/MiComponente.vue'
import MiBoton from './components/MiBoton.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    MiComponente,
    MiBoton
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Titillium+Web&display=swap');

#app {
  font-family: 'Titillium Web', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
