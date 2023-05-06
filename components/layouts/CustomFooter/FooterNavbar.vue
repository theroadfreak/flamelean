<template>
  <div class="container-fluid bg-secondary ">
    <div class="navbar container text-center mx-auto p-4 row d-flex flex-row align-content-center">
      <div v-for="(link, i) in navItems" :key="i" class="col-xxl-3 ">
        <nuxt-link class="text-white text-decoration-none" to="/">{{ link }}</nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterNavbar",
  props: {
    navItems:{
      type: Array,
      default: null
    }
  }
}
</script>

<style scoped>

</style>
