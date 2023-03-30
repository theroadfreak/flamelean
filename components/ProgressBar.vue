<template>
  <div class="w-100 bg-white rounded rounded-2">
    <div class="bg-warning py-1 rounded-start" :class="width">
      <div class="text-secondary text-center">Almost Complete...</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProgressBar",
  props: {
    width: {
      type: String,
      required: true,
    }
  },
}
</script>

<style scoped>

</style>
