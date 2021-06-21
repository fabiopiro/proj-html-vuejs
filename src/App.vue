<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
// components import
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
// components import


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  }
}

</script>

<style lang="scss">
  // general import
  @import './style/general.scss';

  // variables import - !vanno importate per ogni componente!
  @import './style/variables.scss';

</style>
