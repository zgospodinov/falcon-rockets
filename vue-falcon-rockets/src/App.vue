<template>
  <div id="app">
    
    <img alt="Vue logo" src="./assets/rocket.png">
    <SpaceX msg='Hi Falcon'></SpaceX>
  </div>
</template>

<script>
import * as PIXI from 'pixi.js'
import SpaceX from './components/SpaceX.vue'

export default {
  name: 'app',
  components: {
    SpaceX
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
