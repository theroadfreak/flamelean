<template>
  <section class="bg-light">
    <div class="container d-flex justify-content-center py-5">
      <div class="col-12 col-lg-10 d-flex justify-content-between align-items-center">
        <div v-for="(feature, i) in features" :key="i" class="fs-5 custom-font-size-xs text-center fw-bold">
          <div class="text-primary">
            100%
          </div>
          <div class="text-uppercase text-secondary">
            {{ feature }}
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "FeaturesSection",
  data() {
    return {
      features: [
        'Risk free',
        'Safe & Trusted',
        'Secure',
      ]
    }
  }
}
</script>

<style scoped>
@media (max-width: 575.98px) {
  .custom-font-size-xs {
    font-size: 18px !important;
  }
}
</style>
