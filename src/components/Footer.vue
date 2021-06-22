<template>
  <footer>
      <div class="wrapper-75">
          <Nav :navLinks='navLinks' />
        <div class="footer-text">
            <p class="title">Independent professional who works remotely to help with your busines</p>
            <div class="button-one">What is VA ecactly?</div>
            <p class="copyright">
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
// [data-v-65af85a3]


footer {
    color: $color-one;
    background-color: $color-two;
    padding-top: 50px;
    padding-bottom: 100px;
    .footer-text {
        width: 50%;
        .title {
            font-weight: bold;
            font-size: 32px;
            margin-bottom: 40px;
        }
        .copyright {
            font-size: 12px;
            margin-top: 40px;

            a {
                text-decoration: none;
                color: $color-four;
            }
        }
    }
}
</style>