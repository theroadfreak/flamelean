<template>
  <section class="container py-5 text-center">
    <div class="mb-5">
      <h2 class="text-secondary fw-bold mb-5">That’s Right, If You Don’t Think Your New Life Is…</h2>
      <div class="d-flex flex-column align-items-center justify-content-center">
        <div v-for="(feature, i) in features" :key="i" class="mb-3">
          <div>
            <img src="../../assets/images/index/check.svg"
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
    <div>
      <h2 class="text-secondary fw-bold mb-5">This Really Is A Game-Changer!</h2>
      <div v-for="text in textParts" :key="text" class="col-12 d-flex flex-column align-items-center">
        <div class="col-12 col-lg-10 col-xl-8 text-secondary mb-1">
          {{ text }}
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "FlameleanImpactSection",
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
      textParts: [
        'Consider this…',
        `Just ONE of those 4 ingredients would support healthy blood glucose levels and trigger
long-lasting weight loss.`,
        'Now picture uniting all of them in scientifically-proven amounts…',
        `And adding 15 other well-researched botanicals, nutrients, and minerals to boost and accelerate
your transformation even more!`,
        `That's precisely what we've created – and it's the reason our customers are looking
and feeling incredible.`,
      ]
    }
  }
}
</script>

<style scoped>

</style>
