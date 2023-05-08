<template>
  <div class="container d-flex flex-column align-items-center py-4">
    <h1 class="mb-4 fw-bold text-center">{{ title }}</h1>
    <div class="fs-5 w-75">
      {{ text }}
    </div>
  </div>
</template>

<script>
export default {
  name: "TitleText",
  props: {
    title: {
      type: String,
      default: ''
    },
    text: {
      type: String,
      default: '',
    }
  }
}
</script>

<style scoped>

</style>
