<template>
  <div>
    <custom-navbar />
    <nuxt />
  </div>
</template>

<script>
import CustomNavbar from "../components/layouts/CustomNavbar";
export default {
  name: "Default",
  components: {CustomNavbar}
}
</script>

<style scoped>

</style>
