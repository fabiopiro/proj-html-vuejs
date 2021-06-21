<template>
  <header>
      <Nav :navLinks='navLinks'/>
      <div class="wrapper-80">
          <div class="jumbotron d-flex">
              <div id="jumbotron-text">
                  <h1>
                    Indipendent professional who work remotely to help with your business
                  </h1>
                  <h6>
                      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vel fuga quam, iusto enim neque deserunt.
                  </h6>
                  <span class="button-one">
                      What is VA exactly?
                  </span>
              </div>
              <div id="jumbotron-image">
                  <img src="../assets/img/info-1.jpg" alt="">
              </div>
          </div>
      </div>
  </header>
</template>

<script>
// components import
import Nav from './Nav.vue'
// components import

export default {
    name: 'Header',
    components: {
        Nav
    },
    props: {
        navLinks: {
            type: Array,
            required: true,
        },
    }
}
</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';
header {
    // background-color: $color-two;
    background: linear-gradient(
        to bottom,
        $color-two 0%,
        $color-two 90%,
        $color-one 90%,
        $color-one 100%
    );
}
.jumbotron {
    #jumbotron-text,
    #jumbotron-image {
        width: 50%;
    }
    #jumbotron-text {
        text-align: center;
        padding: 5% 0;
        padding-right: 5%;
        color: $color-one;
        h1 {
            font-weight: bold;
            font-size: 50px;
            margin-bottom: 25px;
        }
        h6 {
            margin-bottom: 50px;
        }
    }
    #jumbotron-image {
        padding-left: 5%;
        padding-bottom: 5%;
        img {
            width: 100%;
            border-radius: 5px;
            overflow: hidden;
        }
    }

}
</style>