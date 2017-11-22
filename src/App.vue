<template>
  <div id="app">
    <NavWycode/>
    <router-view/>
  </div>
</template>

<script>
  import NavWycode from './components/NavWycode.vue'

  export default {
    name: 'app',
    components: {
      NavWycode
    }
  }
</script>

<style>
  #app {
    /*font-family: 'Avenir', Helvetica, Arial, sans-serif;*/
    /*-webkit-font-smoothing: antialiased;*/
    /*-moz-osx-font-smoothing: grayscale;*/
    text-align: center;
    /*color: #2c3e50;*/
    /*margin-top: 60px;*/
  }
</style>
