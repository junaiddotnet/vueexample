<template>
  <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld/>
    <HelloWorldone/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import HelloWorldone from './components/HelloWorldone'


export default {
  name: 'App',
  components: {
    HelloWorld,
    HelloWorldone
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
