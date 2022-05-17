<template>
  <div id="app">
    <Header_c />
    <Main_c />
    <Footer_c />
  </div>
</template>

<script>

import Header_c from './components/header_component.vue'
import Main_c from './components/main_component.vue'
import Footer_c from './components/footer_component.vue'

export default {
  name: 'App',
  components: {
    Header_c,
    Main_c,
    Footer_c
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
