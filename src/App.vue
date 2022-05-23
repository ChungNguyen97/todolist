<template>
  <div id="app">
    <header-page />
    <product-page />
    <footer-page />
  </div>
</template>

<script>
import HeaderPage from './components/common/HeaderPage.vue'
import FooterPage from './components/common/FooterPage.vue'
import ProductPage from './pages/ProductPage'

export default {
  name: 'App',
  components: {
    HeaderPage,
    FooterPage,
    ProductPage
  }
}
</script>

<st,
    ProductPageyle>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
}
</style>
