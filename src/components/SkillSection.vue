<template>
  <section>
      <div class="wrapper-75">
        <div class="title">
          <div class="wrapper-75">
            <h5>Lorem ipsum dolor sit amet.</h5>
            <h2>Highly-skilled, independent professional freelancer.</h2>
            <div class="button-two">What is VA exactly?</div>
          </div>
        </div>
        <div class="card-container skill-card-container">
            <div class="container">
            <div class="row">
              <div class="col-lg-4">
                <div class="card-item d-flex">
                  <div class="card-number">
                    <span>1.</span>
                  </div>
                  <div class="card-text">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium, ullam?</p>
                    <a href="">Learn More</a>
                  </div>
                </div>
              </div>
              <div class="col-lg-4">
                <div class="card-item d-flex">
                  <div class="card-number">
                    <span>1.</span>
                  </div>
                  <div class="card-text">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt, atque.</p>
                    <a href="">Learn More</a>
                  </div>
                </div>
              </div>
              <div class="col-lg-4">
                <div class="card-item d-flex">
                  <div class="card-number">
                    <span>1.</span>
                  </div>
                  <div class="card-text">
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corrupti, veniam.</p>
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
    name: 'SkillSection',
}
</script>

<style lang="scss" scoped>
  // variables import
  @import '../style/variables.scss';

  section {
    color: $color-one;
    background-color: $color-two;
    padding: 120px 0;

    .title {
      text-align: center;
      margin: auto;
      margin-bottom: 50px;
    }
  }
</style>