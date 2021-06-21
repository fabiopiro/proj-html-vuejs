<template>
  <div>
      <Nav />
  </div>
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

}
</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';
div {
    height: 500px;
}

</style>