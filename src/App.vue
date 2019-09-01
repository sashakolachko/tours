<template>
<div id="app">
  <Header />
  <Tours />
  <Footer year="2019" />
</div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Tours from './components/Tours.vue'

export default {
  name: 'app',
  components: {
    Header,
    Footer,
    Tours
  }
}
</script>

<style>
#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-family: 'Quicksand', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  overflow: hidden;

}
</style>
