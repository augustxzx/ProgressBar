<template>
  <div id="app">
    <progressbar width="100%" leftColor="linear-gradient(to right, blue, green)" bgColor="#ccc"></progressbar>
  </div>
</template>
<script>
import ProgressBar from './components/ProgressBar.vue'
export default {     
  name: 'App',
  components : {
    progressbar : ProgressBar  
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
}
</style>
