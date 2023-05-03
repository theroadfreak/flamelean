<template>
  <div>
    <div class="d-flex flex-column align-items-center justify-content-center">
      <div v-for="(item, i) in list" :key="i" class="mb-3">
        <div>
          <img src="../assets/images/check.svg"
               width="17"
               height="17"
               alt="Check icon"
               class="me-1"
          />
          {{ item }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FlameleanImpactFeatures",
  props: {
    titleColor: {
      type: String,
      default: 'text-secondary',
    },
    list: {
      type: Array,
      default: null
    }
  }
}
</script>

<style scoped>

</style>
