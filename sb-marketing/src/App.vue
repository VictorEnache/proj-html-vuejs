<template>
  <div id="app">
    <Header_c />
    <Hero_image />
  </div>
</template>

<script>

import Header_c from './components/header_component.vue'
import Hero_image from './components/jumbotron_component.vue'

export default {
  name: 'App',
  components: {
    Header_c,
    Hero_image
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
