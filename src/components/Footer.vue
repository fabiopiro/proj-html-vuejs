<template>
  <footer>
      <div class="wrapper"
        ><Nav :navLinks='navLinks' />
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
footer {
    height: 500px;
    background-color: $color-two;
}

.cont {
    width: 60%;
}

</style>