<template>
  <section class="container mb-5 text-center">
    <flamelean-impacts/>
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
import FlameleanImpactFeatures from "@/components/FlameleanImpactFeatures";
import FlameleanImpacts from "@/components/FlameleanImpacts";
export default {
  name: "FlameleanImpactSection",
  components: {FlameleanImpacts, FlameleanImpactFeatures},
  data() {
    return {
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
