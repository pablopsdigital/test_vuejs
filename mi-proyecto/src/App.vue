<template>
  <div id="app">
    <div class="container">
      <div class="row">
          <mi-menu/>
      </div>
      <div class="row">
        <contenido/>
      </div>
    </div>
  </div>
</template>

<script>
import MiMenu from './components/MiMenu.vue'
import Contenido from './components/Contenido.vue'

export default {
  name: 'App',
  components: {
    MiMenu,
    Contenido
  }
}
</script>

<style>

</style>
