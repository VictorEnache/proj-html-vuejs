<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>

import Header from './components/header_component.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style lang="scss">

@import  './assets/scss/utility.scss';
@import  './assets/scss/common.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  
}
</style>
