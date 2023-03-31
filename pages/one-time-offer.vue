<template>
  <main>
    <hero-section/>
    <best-offer-section/>
  </main>
</template>

<script>
import HeroSection from "@/components/one-time-offer/HeroSection.vue";
import BestOfferSection from "@/components/one-time-offer/BestOfferSection.vue";

export default {
  name: "one-time-offer",
  layout: 'no-navbar',
  components: {BestOfferSection, HeroSection},
  data() {
    return {
      title: 'Best Offer | Flamelean'
    }
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "og:title",
          property: "og:title",
          content: this.title,
        },
      ],
    };
  },
}
</script>

<style scoped>

</style>
