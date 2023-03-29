<template>
  <div class="d-flex flex-column">
    <div v-for="(feature, i) in features" :key="feature"
         class="d-flex align-items-center"
         :class="{ 'mb-4' : i !== features.length - 1 }">
      <img src="../../../assets/images/index/flamelean-features/like-icon.svg"
           alt="Like Icon"
           width="60"
           height="60"
           class="me-3"
      />
      <span class="text-secondary">{{ feature }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Feature",
  props: {
    features: {
      type: Array,
      required: true,
    }
  }
}
</script>

<style scoped>

</style>
