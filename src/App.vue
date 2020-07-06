<template>
  <div id="app">
    <Header />
    <router-view />
  </div>
</template>

<script>

import Header from './components/Header'

export default {
  name: 'App',
  components: {
    Header
  },
}
</script>

<style>

  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap');

  #app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    height: 100vh;
  }

  * {
    margin: 0;
    padding: 0;
    font-family: 'Roboto', sans-serif;
  }

  body {
    background-color: #252C4A;
    color: #fff;
  }
</style>
