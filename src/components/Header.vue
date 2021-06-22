<template>
  <header>
      <div class="wrapper-90">
        <Nav :navLinks='navLinks'/>
      </div>
      <div class="wrapper-80">
          <div class="jumbotron d-flex">
              <div id="jumbotron-text">
                  <h2>
                    Indipendent professional who works remotely to help with your business
                  </h2>
                  <h5>
                      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vel fuga quam, iusto enim neque deserunt.
                  </h5>
                  <span class="button-one">
                      What is VA exactly?
                  </span>
              </div>
              <div id="jumbotron-image">
                  <img  class="big-image" src="../assets/img/info-1.jpg" alt="">
              </div>
          </div>
      </div>
      <div class="fixed-container">
          <div class="fixed-text">
              <span>This is a free HubSpot live chat. You can create your own chat flows and engage your customers with Avada & HubSpot!</span>
              <img class="fixed-icon" src="../assets/img/logo.png" alt="">
          </div>
          <div class="fixed-icon-message d-flex justify-content-end">
              <i class="fas fa-comment"></i>
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
        margin: auto;
        // padding: 5% 0;
        // padding-right: 5%;
        color: $color-one;
        h6 {
            margin-bottom: 50px;
        }
    }
    #jumbotron-image {
        padding-left: 5%;
        padding-bottom: 5%;
        img {
            border-radius: 5px;
            overflow: hidden;
        }
    }

}

.fixed-container {
    position: fixed;
    bottom: 2%;
    right: 2%;
    width: 200px;

    .fixed-text {
        padding: 0 15px;
        padding-top: 30px;
        padding-bottom: 10px;
        box-shadow: 1px 1px lightgrey;
        border-radius: 5px;
        background-color: $color-one;
        line-height: 1.2;

        .fixed-icon {
            width: 40px;
            height: 40px;
            position: absolute;
            top: 0;
            left: 50%;
            transform: translate( -50% , -50%);
        }
        span {
            font-size: 12px;
        }
    }
    .fixed-icon-message {
        i {
            font-size: 25px;
            padding: 10px 10px;
            margin-top: 15px;
            color: $color-one;
            background-color: $color-four;
            border-radius: 50%;
        }
    }

}
</style>