<template>
  <div id="app">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld00.vue'
import Rellax from 'rellax'

export default {
  name: 'app',
  components: {
    HelloWorld
  },
  mounted: function() {
    //var rellax = new Rellax('.rellax');
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  background: url('./assets/sushi.svg') no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  height: 100vh; width: 100vw;
  margin: 0;
}
html {
  background-color: #B6FFF4;
}
</style>
