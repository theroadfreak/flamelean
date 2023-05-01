<template>
  <main>
    <hero-section/>
    <last-product-offer-section/>
    <features-section/>
    <next-step/>
  </main>
</template>

<script>
import HeroSection from "@/components/claim-your-discount/HeroSection.vue";
import LastProductOfferSection from "@/components/claim-your-discount/ProductOfferSection.vue";
import FeaturesSection from "@/components/claim-your-discount/FeaturesSection";
import NextStep from "@/components/claim-your-discount/NextStep.vue";

export default {
  name: "claim-your-discount",
  layout: 'no-navbar',
  components: {NextStep, FeaturesSection, LastProductOfferSection, HeroSection},
  data() {
    return {
      title: 'Amazing Discount | Flamelean',
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
