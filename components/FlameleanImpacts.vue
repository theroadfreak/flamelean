<template>
  <section class="container d-flex flex-column align-items-center text-secondary text-center py-5" id="flameleanImpacts">
    <flamelean-impact-features title-color="text-black"
                               :features="features"
                               title="That’s Right, If You Don’t Think Your New Life Is…"
    />
  </section>
</template>

<script>
import FlameleanImpactFeatures from "@/components/FlameleanImpactFeatures";
export default {
  name: "FlameleanImpacts",
  components: {FlameleanImpactFeatures},
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
      ]
    }
  }
}
</script>

<style scoped>

</style>
