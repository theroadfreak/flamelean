<template>
  <main>
    <hero-section/>
    <intro/>
    <the-biggest-suspect-section/>
    <jessica-richards-section/>
    <thing-that-switches-on-fat-burning-section/>
    <why-we-created-flamelean-section/>
    <offer-section :bg-color="true"/>
    <pricing-section :user-review="true"/>
    <frequently-asked-questions-section/>
    <pricing-section :user-review="true"/>
  </main>
</template>

<script>
import HeroSection from "@/components/HeroSection";
import Intro from "@/components/tsl/Intro";
import TheBiggestSuspectSection from "@/components/tsl/TheBiggestSuspectSection";
import JessicaRichardsSection from "@/components/tsl/JessicaRichardsSection";
import ThingThatSwitchesOnFatBurningSection from "@/components/tsl/ThingThatSwitchesOnFatBurningSection";
import WhyWeCreatedFlameleanSection from "@/components/tsl/WhyWeCreatedFlameleanSection";
import PricingSection from "@/components/index/PricingSection";
import FrequentlyAskedQuestionsSection from "@/components/index/FrequentlyAskedQuestionsSection";
import OfferSection from "@/components/index/OfferSection";

export default {
  name: "tsl",
  components: {
    OfferSection,
    FrequentlyAskedQuestionsSection,
    PricingSection,
    WhyWeCreatedFlameleanSection,
    ThingThatSwitchesOnFatBurningSection,
    JessicaRichardsSection, TheBiggestSuspectSection, Intro, HeroSection
  },
  data() {
    return {
      title: 'TSL | Flamelean',
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
