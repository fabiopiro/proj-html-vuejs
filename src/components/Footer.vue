<template>
  <footer>
      <div class="wrapper-75">
          <!-- NAV COMPONENT -->
          <!-- prop
          navLinks -->
          <Nav 
          :navLinks='navLinks' />
          <!-- NAV COMPONENT -->

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
      <!-- button on top -->
      <div class="on-top-button">
          <a href="#"><i class="fas fa-chevron-up"></i></a>
      </div>
      <!-- button in top -->
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
    // prop
    // navLinks from App
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
::v-deep .button-one {
    color: $color-one;
    background-color: $color-three;
    &:hover {
        color: $color-three;
        background-color: $color-one;
    }
}
.button-one {
    color: $color-three;
    background-color: $color-one;
    &:hover {
        color: $color-one;
        background-color: $color-three;
    }
}

footer {
    position: relative;

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
    .on-top-button {
        display: flex;
        justify-content: center;
        align-items: center;

        position: absolute;
        bottom: 0;
        left: 2%;

        width: 40px;
        height: 30px;
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;

        background-color: #2f3038;

        a {
            color: $color-one;
        }
    }
}
</style>