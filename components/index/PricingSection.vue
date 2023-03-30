<template>
  <section class="bg-primary">
    <div class="container py-5 d-flex flex-column align-items-center">
      <h2 class="text-white text-center fw-bold mb-5">Claim your discounted Flamelean<br class="d-none d-sm-flex"/>
        Below While Stocks Last
      </h2>
      <div class="col-12">
        <div class="row d-flex justify-content-center">
          <div v-for="(card, i) in cards" :key="card.bottlePrice"
               class="col-10 col-sm-8 col-md-6 col-lg-4 col-xl-3"
               :class="{ 'mb-4 mb-lg-0 me-md-1 me-lg-0' : i !== cards.length - 1 }"
          >
            <card :card="card"/>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Card from "@/components/index/PricingSection/Card.vue";

export default {
  name: "PricingSection",
  components: {Card},
  data() {
    return {
      cards: [
        {
          quantity: 1,
          supplyDays: 30,
          image: 'flamelean-bottle.png',
          alt: 'Flamelean Bottle',
          bottlePrice: 59,
          initialSumPrice: 300,
          discountedSumPrice: 150,
          freeBonuses: false,
          freeShipping: false,
        },
        {
          quantity: 6,
          supplyDays: 180,
          image: 'flamelean-6-bottles.png',
          alt: 'Flamelean 6 Bottles',
          bottlePrice: 39,
          initialSumPrice: 300,
          discountedSumPrice: 150,
          freeBonuses: true,
          freeShipping: true,
        },
        {
          quantity: 3,
          supplyDays: 90,
          image: 'flamelean-3-bottles.png',
          alt: 'Flamelean 3 Bottles',
          bottlePrice: 49,
          initialSumPrice: 300,
          discountedSumPrice: 150,
          freeBonuses: true,
          freeShipping: false,
        },
      ]
    }
  }
}
</script>

<style scoped>

</style>
