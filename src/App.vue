<template>
  <div id="app">
    <router-view></router-view>
    <page-background></page-background>
  </div>
</template>

<script>
import PageBackground from './components/PageBackground.vue'

export default {
  components: {
    PageBackground
  },
  name: 'app'
}
</script>

<style>

  html, body, div {
    padding: 0px;
    margin: 0px;
  }

  #app {
    padding: 0px;
    margin: 0px;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  .container {
    max-width: 1240px;
    padding: 40px 10px;
  }

  @media (min-width: 992px) {
  .container {
    padding: 40px 140px;
    }
  }

  hr {
    border-color: #e0e0e0;
  }
</style>
