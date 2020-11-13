<template>
  <Nav />
  <Slider />
  <Catalog />
</template>

<script>

import Catalog from './components/catalog.vue'
import Nav from './components/navigation.vue'
import Slider from './components/slider.vue'


export default {
  name: 'App',
  components: {
    Catalog,
    Nav,
    Slider,
  }
}
</script>

<style>
#app {
  font-family: Inter, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #000;
}
</style>
