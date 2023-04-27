<template>
  <main>
    <hero-section/>
    <the-blood-sugar-secret/>
    <flamelean-carnitine-substance-section id="about-flamelean"/>
    <flamelean-ingredients-section id="ingredients"/>
    <flamelean-features-section/>
    <offer-section/>
    <shipping-section/>
    <reviews-section/>
    <pricing-section/>
    <money-back-guarantee-section/>
    <frequently-asked-questions-section id="faq"/>
  </main>
</template>

<script>
import HeroSection from "@/components/index/HeroSection.vue";
import FlameleanCarnitineSubstanceSection from "@/components/index/FlameleanCarnitineSubstanceSection.vue";
import FlameleanIngredientsSection from "@/components/index/FlameleanIngredientsSection.vue";
import FlameleanFeaturesSection from "@/components/index/FlameleanFeaturesSection.vue";
import OfferSection from "@/components/index/OfferSection.vue";
import ShippingSection from "@/components/index/ShippingSection.vue";
import ReviewsSection from "@/components/index/ReviewsSection.vue";
import PricingSection from "@/components/index/PricingSection.vue";
import MoneyBackGuaranteeSection from "@/components/index/MoneyBackGuaranteeSection.vue";
import FrequentlyAskedQuestionsSection from "@/components/index/FrequentlyAskedQuestionsSection.vue";
import TheBloodSugarSecret from "@/components/index/TheBloodSugarSecret.vue";

export default {
  name: 'IndexPage',
  components: {
    TheBloodSugarSecret,
    FrequentlyAskedQuestionsSection,
    MoneyBackGuaranteeSection,
    PricingSection,
    ReviewsSection,
    ShippingSection,
    OfferSection,
    FlameleanFeaturesSection,
    FlameleanIngredientsSection,
    FlameleanCarnitineSubstanceSection, HeroSection
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
