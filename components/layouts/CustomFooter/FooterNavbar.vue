<template>
  <div class="navbar bg-secondary container-fluid justify-content-between p-4">
    <div v-for="(link, i) in navItems" :key="i" class="d-flex flex-row nav-item">
      <nuxt-link class=" text-white text-decoration-none" to="/">{{ link }}</nuxt-link>
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
