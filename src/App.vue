<template>
  <div id="app">    
    <login-component></login-component>
  </div>
</template>

<script>
import LoginComponent from './components/LoginComponent'

export default {
  name: 'App',
  components: {
    LoginComponent
  }
}
</script>

<style lang="less">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
