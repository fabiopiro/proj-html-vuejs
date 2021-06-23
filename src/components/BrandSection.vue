<template>
  <section>
      <div class="wrapper-75">
        <h6 class="text-center">Trusted by this amazing brands</h6>
        <div class="brand-list">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <img src="../assets/img/brand-1.jpg" alt="">
                    </div>
                    <div class="col">
                        <img src="../assets/img/brand-2.jpg" alt="">
                    </div>
                    <div class="col">
                        <img src="../assets/img/brand-3.jpg" alt="">
                    </div>
                    <div class="col">
                        <img src="../assets/img/brand-4.jpg" alt="">
                    </div>
                    <div class="col">
                        <img src="../assets/img/brand-5.jpg" alt="">
                    </div>
                    
                </div>
            </div>
        </div>
        <div class="brand-main d-flex">
            <div id="brand-main-text">
                <img class="icon" src="../assets/img/icon-2.png" alt="">
                <h3>Professional who works to help with your business</h3>
                <h5>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eligendi modi obcaecati eos doloremque officia deleniti.</h5>
                <div class="button-two">What is VA exactly?</div>
            </div>
            <div id="brand-main-image">
                <img class="big-image" src="../assets/img/info-3.png" alt="">
            </div>
        </div>
        <div class="card-container brand-card-container">
            <div class="container">
            <div class="row">
              <div class="col-lg-6">
                <div class="card-item-two d-flex">
                  <div class="card-number">
                    <span>1.</span>
                  </div>
                  <div class="card-text">
                    <h5>Learn to delegate</h5>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Doloribus inventore eveniet animi sint quaerat libero. Modi illum id veniam est.</p>
                    <a href="">Learn More</a>
                  </div>
                </div>
              </div>
              <div class="col-lg-6">
                <div class="card-item-two d-flex">
                  <div class="card-number">
                    <span>1.</span>
                  </div>
                  <div class="card-text">
                    <h5>Reduce labor cost</h5>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Maiores, qui. Excepturi eum rem itaque accusantium ab. Commodi nesciunt maiores hic?</p>
                    <a href="">Learn More</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'BrandSection',
}
</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';

    section {
        margin: 120px 0;
        background-color: $color-one;
        color: $color-two;
    }
    .brand-list {
        img {
            width: 100%;
        }
    }
    .brand-main {
        margin: 50px 0;
        #brand-main-text,
        #brand-main-image {
            width: 50%;
        }
        #brand-main-text {
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
          }
    }
</style>