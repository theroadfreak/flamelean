<template>
  <main>
    <hero-section/>
    <the-blood-sugar-secret-section/>
    <pricing-section/>
    <flamelean-ingredients-section id="ingredients"/>
    <flamelean-features-section/>
    <offer-section/>
    <shipping-section/>
    <reviews-section/>
    <money-back-guarantee-section/>
    <frequently-asked-questions-section id="faq"/>
  </main>
</template>

<script>
import HeroSection from "@/components/index/HeroSection.vue";
import FlameleanIngredientsSection from "@/components/index/FlameleanIngredientsSection.vue";
import FlameleanFeaturesSection from "@/components/index/FlameleanFeaturesSection.vue";
import OfferSection from "@/components/index/OfferSection.vue";
import ShippingSection from "@/components/index/ShippingSection.vue";
import ReviewsSection from "@/components/index/ReviewsSection.vue";
import PricingSection from "@/components/index/PricingSection.vue";
import MoneyBackGuaranteeSection from "@/components/index/MoneyBackGuaranteeSection.vue";
import FrequentlyAskedQuestionsSection from "@/components/index/FrequentlyAskedQuestionsSection.vue";
import TheBloodSugarSecretSection from "@/components/index/TheBloodSugarSecretSection.vue";

export default {
  name: 'IndexPage',
  components: {
    TheBloodSugarSecretSection,
    FrequentlyAskedQuestionsSection,
    MoneyBackGuaranteeSection,
    PricingSection,
    ReviewsSection,
    ShippingSection,
    OfferSection,
    FlameleanFeaturesSection,
    FlameleanIngredientsSection,
    HeroSection
  },
  data() {
    return {
      title: 'Homepage | Flamelean',
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
