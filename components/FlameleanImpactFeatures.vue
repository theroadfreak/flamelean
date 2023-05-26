<template>
  <div>
    <h2 class="text-center fw-bold mb-5" :class="titleColor">
      {{ title }}
    </h2>
    <div
      class="d-flex flex-column text-center align-items-center justify-content-center"
    >
      <div v-for="(feature, i) in features" :key="i" class="mb-3">
        <div class="text-secondary">
          <img
            src="../assets/images/check.svg"
            width="17"
            height="17"
            alt="Check icon"
            class="me-1"
          />
          {{ feature }}
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
      default: "text-secondary",
    },
    features: {
      type: Array,
      default: null,
    },
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped></style>
