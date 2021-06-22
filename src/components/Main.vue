<template>
  <div>
    <ServiceSection />
    <SkillSection />
    <BrandSection />
  </div>
</template>

<script>
import ServiceSection from './ServiceSection.vue'
import SkillSection from './SkillSection.vue'
import BrandSection from './BrandSection.vue'


export default {
    name: 'Main',
    components: {
        ServiceSection,
        SkillSection,
        BrandSection,
    }

}
</script>

<style lang="scss" scoped>
// variables import
@import '../style/variables.scss';

</style>