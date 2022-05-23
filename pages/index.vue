<template>
  <div>
    <Banner />
    <TheResort />
    <TheStay />
    <DinnerJannata />
    <Review />
  </div>
</template>

<style scoped>

</style>

<script>
import Banner from '~/components/Banner.vue'
import TheResort from '~/components/TheResort.vue'
import DinnerJannata from '~/components/DinnerJannata.vue'
import Review from '../components/Review.vue'
import TheStay from '../components/TheStay.vue'
export default {
  name: 'IndexPage',
  components: { Banner, TheResort, TheStay, DinnerJannata, Review },
}
</script>
