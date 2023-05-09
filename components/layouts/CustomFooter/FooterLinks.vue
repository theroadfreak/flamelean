<template>
  <div class="py-4">
    <div class="container d-flex justify-content-center">
      <div class="col-12 col-lg-11 d-flex flex-column flex-sm-row align-items-center justify-content-sm-between">
        <div v-for="(link, i) in footerLinks" :key="i" :class="{ 'mb-3 mb-sm-0' : i !== footerLinks.length - 1 }">
          <nuxt-link v-if="link.link" class="text-white text-decoration-none small" :to="link.link">{{ link.name }}</nuxt-link>
          <a class="text-white text-decoration-none small" v-if="link.href" :href= link.href target="_blank">{{ link.name }}</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterLinks",
  props: {
    footerLinks: {
      type: Array,
      default: null
    }
  }
}
</script>

<style scoped>

</style>
