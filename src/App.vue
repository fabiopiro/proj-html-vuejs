<template>
  <div id="app">
    <Header :navLinks='navLinks' />
    <Main />
    <Footer :navLinks='navLinks' />
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
  },
  data: function () {
    return {
      navLinks: [
          {
            name: 'home',
            link: '#'
          },
          {
            name: 'about',
            link: '#'
          },
          {
            name: 'services',
            link: '#'
          },
          {
            name: 'journal',
            link: '#'
          },
          {
            name: 'contacts',
            link: '#'
          },
      ],
    }
  },
}

</script>

<style lang="scss">
  // general import
  @import './style/general.scss';

  // variables import - !vanno importate per ogni componente!
  @import './style/variables.scss';

</style>
