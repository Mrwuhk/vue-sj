<template>
  <div id="app">
  
    <router-view></router-view>
  </div>
</template>

<script>

export default {
  name: 'app',
  components: {

  }
}
</script>

<style>
* {
  margin:0;
  padding: 0;
  box-sizing: inherit;
}
#app {
  width: 100vw;
  height: 100vh;
  box-sizing: border-box;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;

}
</style>

