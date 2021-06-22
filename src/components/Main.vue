<template>
  <div>
      <div class="container w-75">
        <section class="section-one">
            <h5>Available services</h5>
            <div class="services d-flex">
                <div class="services-item">
                    <h4>Answering phone calls</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>
                <div class="services-item">
                    <h4>Answering phone calls</h4>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                </div>
                <div class="services-item">
                    <h4>Answering phone calls</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>
                <div class="services-item">
                    <h4>Answering phone calls</h4>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                </div>
            </div>
            <div class="virtual-assistant d-flex">
                <div id="virtual-assistant-image">
                    <img class="big-image" src="../assets/img/info-2.png" alt="">
                </div>
                <div id="virtual-assistant-info">
                    <img class="icon" src="../assets/img/icon-1.png" alt="">
                    <h3>Find the ultimate virtual assistant for your business</h3>
                    <h6>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora consequatur, fuga sit laudantium vitae iste?</h6>
                    <span class="button-two">What is VA exactly</span>
                </div>
            </div>
        </section>

        <section class="section-three">

        </section>  
      </div>
        <SkillSection />
        <BrandSection />
  </div>
</template>

<script>
import SkillSection from './SkillSection.vue'
import BrandSection from './BrandSection.vue'


export default {
    name: 'Main',
    components: {
        SkillSection,
        BrandSection,
    }

}
</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';

.section-one {
    margin: 15px 0;
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
        }
    }
    .virtual-assistant {
        margin: 50px 0;
        #virtual-assistant-image,
        #virtual-assistant-info {
            width: 50%;
        }
        
        #virtual-assistant-info {
            color: $color-three;
            text-align: center;
            margin: auto;

            h6 {
                color: $color-three;
                font-weight: 400;
                margin-bottom: 30px;

            }
        }
    }
}

</style>