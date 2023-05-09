<template>
  <div class="text-center">
    <nuxt-link :to="{ name: 'index' }" class="btn btn-light px-3 btn-outline-primary fs-4 rounded rounded-3 shadow-lg">
      <b>Click <u>HERE</u> To Discover More About FlameLean</b><br>
      And Reveal Special Discounted Offers!
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: "DiscountedOffersButton"
}
</script>

<style scoped>

</style>
