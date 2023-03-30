<template>
  <main>
    <hero-section/>
    <last-product-offer-section/>
  </main>
</template>

<script>
import HeroSection from "@/components/last-offer/HeroSection.vue";
import LastProductOfferSection from "@/components/last-offer/LastProductOfferSection.vue";

export default {
  name: "last-offer",
  components: {LastProductOfferSection, HeroSection},
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
