<template>
<section>
    <div class="container w-75">
        <section class="service-section">
            <h6>Available services</h6>
            <div class="services d-flex">
                <div class="services-item">
                    <h4>Answering phone calls</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>
                <div class="services-item">
                    <h4>Basic data entry</h4>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                </div>
                <div class="services-item">
                    <h4>Organizing calendar</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>
                <div class="services-item">
                    <h4>Booking travels</h4>
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
                    <h5>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora consequatur.</h5>
                    <span class="button-two">What is VA exactly</span>
                </div>
            </div>
        </section>
      </div>
</section>
</template>

<script>

export default {
    name: 'ServiceSection',
}

</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';

section {
    background-color: $color-one;
}

.service-section {
    margin: 15px 0;
    .services {
        color: $color-two;
        margin-bottom: 15px;
        .services-item {
            width: 25%;
            padding: 5% 5%;
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
            color: $color-two;
            text-align: center;

            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
    }
}
</style>