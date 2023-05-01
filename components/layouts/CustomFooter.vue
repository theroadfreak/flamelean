<template>
  <div class="bg-primary">
    <div class="container d-flex flex-column align-items-center py-5">
      <nuxt-link to="/" class="mb-5">
        <img
          src="../../assets/images/layouts/logo.svg"
          alt="Flamelean's Logo"
          width="150"
          height="34"
        />
      </nuxt-link>
      <div class="text-white text-center fs-5">
        FlameLean is not endorsed by, sponsored by, or<br class="d-none d-sm-flex"/>
        affiliated with any of these organizations.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CustomFooter"
}
</script>

<style scoped>

</style>
