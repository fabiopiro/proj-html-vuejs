<template>
    <header>
        <!-- SIDE ICONS -->
        <div class="header-icons-container">
            <div class="header-icon">
                <i class="far fa-folder"></i>
                <span>Demos</span>
            </div>
            <div class="header-icon">
                <div class="dollar d-flex justify-content-center">
                    <span class="dollar-symbol">$</span>
                    <span class="dollar-number">39</span>
                </div>
                <span>On Sale</span>
            </div>
        </div>
        <!-- /SIDE ICONS -->
        <div class="wrapper-95">
            <!-- NAV COMPONENT-->
            <!-- prop navLinks -->
            <Nav :navLinks='navLinks'/>
            <!-- /NAV COMPONENT-->
        </div>
        <!-- JUMBOTRON -->
        <div class="wrapper-80">
            <div class="jumbotron d-flex">
                <!-- jumbotron text -->
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
                <!-- /jumbotron text -->
                <!-- jumbotron image -->
                <div id="jumbotron-image">
                  <img  class="big-image" src="../assets/img/info-1.jpg" alt="">
                </div>
                <!-- /jumbotron image -->
            </div>
        </div>
        <!-- /JUMBOTRON -->
        <!-- FIXED CHAT -->
        <div class="fixed-container">
            <div
            v-if="!isHidden"
            class="fixed-text">
              <i
              @click="isHidden = true"
              class="fas fa-times"></i>
              <span>This is a free HubSpot live chat. You can create your own chat flows and engage your customers with Avada & HubSpot!</span>
              <img class="fixed-icon" src="../assets/img/logo.png" alt="">
            </div>
             <div class="fixed-icon-message d-flex justify-content-end">
              <i
              @click="isHidden = false"
              class="fas fa-comment"></i>
            </div>
        </div>
        <!-- /FIXED CHAT -->
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
    // prop
    // navLinks from App
    props: {
        navLinks: {
            type: Array,
            required: true,
        },
    },
    data: function () {
        return {
            isHidden: false,
        }
    }
}

</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';

header {
    position: relative;
    background: linear-gradient(
        to bottom,
        $color-two 0%,
        $color-two 90%,
        $color-one 90%,
        $color-one 100%
    );
    
    // SIDE ICONS
    .header-icons-container {
        position: absolute;
        top: 15%;
        right: 1%;
        .header-icon {
            position: relative;

            display: flex;
            flex-direction: column;
            justify-content: space-evenly;

            text-align: center;
            font-size: 10px;
            width: 50px;
            height: 50px;
            margin-bottom: 5px;
            background-color: $color-one;
            border-radius: 5px;
            box-shadow: 1px 1px lightgrey;
            cursor: pointer;

            i {
                font-size: 20px;
            }

            .dollar {
                color: #90cd9b;
                font-weight: bold;
                .dollar-symbol {
                    font-size: 15px;
                }
                .dollar-number {
                    font-size: 22px;
                }
            }
        }
    }
    // /SIDE ICONS
}
// JUMBOTRON
.jumbotron {
    #jumbotron-text,
    #jumbotron-image {
        width: 50%;
    }
    #jumbotron-text {
        text-align: center;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        color: $color-one;

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
// /JUMBOTRON

// FIXED CHAT
.fixed-container {
    position: fixed;
    bottom: 2%;
    right: 2%;
    width: 200px;

    z-index: 99;

    .fixed-text {
        padding: 0 15px;
        padding-top: 30px;
        padding-bottom: 10px;
        // box-shadow: 1px 1px lightgrey;
        -webkit-box-shadow: 0 0 2px lightgrey;
        box-shadow: 0 0 2px lightgrey;
        border-radius: 5px;
        background-color: $color-one;
        line-height: 1.2;

        i {
            position: absolute;
            top: 5px;
            right: 5px;
            cursor: pointer;
            color: lightgrey;
        }

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
            cursor: pointer;
        }
    }
}
// / FIXED CHAT
</style>