<template>
  <div id="app">
  	<test></test>
  	<otext></otext>
  </div>
</template>

<script>
import Test from './components/test'
import Otext from './components/otext'
export default {
  name: 'app',
  components: {Test,Otext}
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
