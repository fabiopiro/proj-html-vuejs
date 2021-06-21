<template>
  <div>
      <div class="container w-75">
        <section class="section-one">
            <h6>Available services</h6>
            <div class="services d-flex">
                <div class="services-item">
                    <h3>Answering phone calls</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed, debitis.</p>
                </div>
                <div class="services-item">
                    <h3>Answering phone calls</h3>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                </div>
                <div class="services-item">
                    <h3>Answering phone calls</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>
                <div class="services-item">
                    <h3>Answering phone calls</h3>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                </div>
            </div>
            <div class="virtual-assistant d-flex">
                <div id="virtual-assistant-image">
                    <img src="../assets/img/info-2.png" alt="">
                </div>
                <div id="virtual-assistant-info">
                    <img src="../assets/img/icon-1.png" alt="">
                    <h2>Find the ultimate virtual assistant for your business</h2>
                    <h6>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nam, repellat?</h6>
                    <span class="button-two">What is VA exactly</span>
                </div>
            </div>
        </section>
        <section class="section-two">

        </section>
        <section class="section-three">

        </section>  
      </div>
  </div>
</template>

<script>
export default {
    name: 'Main'

}
</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';

.section-one {
    margin: 15px 0;
    h6 {
        color: $color-four;
        font-weight: bold;
        margin-bottom: 20px;
    }
    .services {
        color: $color-three;
        margin-bottom: 15px;
        .services-item {
            width: 25%;
            padding: 3% 5%;
            border-top: 2px solid lightgrey;
            &:not(:nth-child(4)) {
                border-right: 2px solid lightgrey;
            }
            h3 {
                font-weight: bold;
            }
        }
    }
    .virtual-assistant {
        #virtual-assistant-image,
        #virtual-assistant-info {
            width: 50%;
        }
        #virtual-assistant-image {
            img {
                width: 100%;
            }
        }
        #virtual-assistant-info {
            color: $color-three;
            text-align: center;
            margin: auto;
            img {
                width: 150px;
            }
            h2 {
                font-weight: bold;
            }
            h6 {
                color: $color-three;
                font-weight: 400;
            }
        }
    }
}

</style>