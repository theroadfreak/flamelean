<template>
  <main>
    <hero-section/>
    <stanford-scientists-article-section/>
    <flamelean-carnitine-substance-section/>
    <flamelean-ingredients-section/>
    <flamelean-features-section/>
    <offer-section/>
    <shipping-section/>
    <reviews-section/>
    <pricing-section/>
  </main>
</template>

<script>
import HeroSection from "@/components/index/HeroSection.vue";
import StanfordScientistsArticleSection from "@/components/index/StanfordScientistsArticleSection.vue";
import FlameleanCarnitineSubstanceSection from "@/components/index/FlameleanCarnitineSubstanceSection.vue";
import FlameleanIngredientsSection from "@/components/index/FlameleanIngredientsSection.vue";
import FlameleanFeaturesSection from "@/components/index/FlameleanFeaturesSection.vue";
import OfferSection from "@/components/index/OfferSection.vue";
import ShippingSection from "@/components/index/ShippingSection.vue";
import ReviewsSection from "@/components/index/ReviewsSection.vue";
import PricingSection from "@/components/index/PricingSection.vue";

export default {
  name: 'IndexPage',
  components: {
    PricingSection,
    ReviewsSection,
    ShippingSection,
    OfferSection,
    FlameleanFeaturesSection,
    FlameleanIngredientsSection,
    FlameleanCarnitineSubstanceSection, StanfordScientistsArticleSection, HeroSection
  }
}
</script>
