<template>
  <img alt="Maintainance" src="./assets/main.png">
  <HelloWorld msg="Whats up man?" email="njaneambrose@gmail.com"/>
  <SimpleCalc hi="See me............helllo" cl="myclassA" isdsb=""/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import SimpleCalc from './components/SimpleCalc.vue'

export default {
  name: 'App',
  components: {
    HelloWorld, SimpleCalc
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
