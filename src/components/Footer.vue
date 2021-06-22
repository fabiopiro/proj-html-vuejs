<template>
  <footer>
      <div class="wrapper-75"
        ><Nav :navLinks='navLinks' />
        <div class="footer-text">
            <h3>Independent professional who works remotely to help with your busines</h3>
            <div class="button-one">What is VA ecactly?</div>
            <p>
                <i class="far fa-copyright"></i>
                Copyright 2012 - 2020 | Avada Theme by
                <a href="">Theme Fusion</a>
                | All right reserved
                | Powered by
                <a href="">Wordpress</a>
            </p>
        </div>
      </div>
  </footer>
</template>

<script>
// components import
import Nav from './Nav.vue'
// components import

export default {
    name: 'Footer',
    components: {
        Nav
    },
    props: {
        navLinks: {
            type: Array,
            required: true,
        },
    },

}
</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';
footer {
    height: 500px;
    background-color: $color-two;
}



</style>