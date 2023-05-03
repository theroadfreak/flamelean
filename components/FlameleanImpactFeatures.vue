<template>
  <div>
    <h2 class="text-center fw-bold mb-5" :class="titleColor">That’s Right, If You Don’t Think Your New Life Is…</h2>
    <div class="d-flex flex-column align-items-center justify-content-center">
      <div v-for="(feature, i) in features" :key="i" class="mb-3">
        <div>
          <img src="../assets/images/check.svg"
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
      default: 'text-secondary',
    }
  },
  data() {
    return {
      features: [
        'Stress-free now your blood glucose levels are stable and rarely spike or crash',
        'A breeze now your body is able to use insulin more effectively, naturally',
        'Joyful because you’re no longer fighting a losing battle against carb and sugar cravings',
        'Energetic now the herbal blend is giving you a natural boost',
        'Super easy to lose weight because you’re fuller for longer and actually enjoy being active',
        'Empowering every time you’re told: “wow, you’ve lost so much weight - you look great!”',
        'The best it’s ever been now you’re finally in control of your blood sugar and weight…',
      ],
    }
  }
}
</script>

<style scoped>

</style>
