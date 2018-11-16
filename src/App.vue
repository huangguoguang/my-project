<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!-- <Parent></Parent> -->
    <!-- <Parents></Parents> -->
    <Parentss></Parentss>
  </div>
</template>

<script>

import Parent from './components/Parent'
import Parents from './components/slots/Parent'
import Parentss from './components/dongtaizujian/Parent'

export default {
  name: 'App',
  components: {
    Parent,
    Parents,
    Parentss
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
