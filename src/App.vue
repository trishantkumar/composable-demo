<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld />
  <h1>Below we have composition API code - </h1>
  <HelloWorldComp />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HelloWorldComp from './components/HelloWorldComposition.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    HelloWorldComp
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
