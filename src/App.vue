<template>
  <div id="app">
    <img src="./assets/logo.png">
    <my-component></my-component>
    <router-view></router-view>
  </div>
</template>

<script>

  var Child = {
    template: '<div>A custom component!</div>'
  }

  export default {
  name: 'app',
    components: {
    'my-component':Child,
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
