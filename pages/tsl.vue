<template>
  <main>
    <hero-section/>
    <intro/>
    <the-biggest-suspect-section/>
    <jessica-richards-section/>
    <thing-that-switches-on-fat-burning-section/>
    <common-side-effects-section/>
    <medication-consequences-section/>
    <the-most-important-thing-section/>
    <why-we-created-flamelean-section id="about-flamelean"/>
    <four-star-of-the-show-section/>
    <natural-solution-section/>
    <flamelean-ingredients-section/>
    <links/>
    <plant-based-remedies-section/>
    <pricing-section :stock-available-text="true"/>
    <offer-section :bg-color="true"/>
    <pricing-section :user-review="true" :free-shipping-title="true"/>
    <money-back-guarantee-section/>
    <pricing-section :user-review="true" :free-shipping-title="true"/>
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
import FourStarOfTheShowSection from "@/components/tsl/FourStarOfTheShowSection";
import NaturalSolutionSection from "@/components/tsl/NaturalSolutionSection";
import FlameleanIngredientsSection from "@/components/FlameleanIngredientsSection";
import Links from "@/components/tsl/Links";
import PlantBasedRemediesSection from "@/components/tsl/PlantBasedRemediesSection";
import MoneyBackGuaranteeSection from "@/components/tsl/MoneyBackGuaranteeSection";
import CommonSideEffectsSection from "~/components/tsl/CommonSideEffectsSection";
import TheMostImportantThingSection from "~/components/tsl/TheMostImportantThingSection";
import MedicationConsequencesSection from "~/components/tsl/MedicationConsequencesSection";

export default {
  name: "tsl",
  components: {
    TheMostImportantThingSection,
    MedicationConsequencesSection,
    CommonSideEffectsSection,
    MoneyBackGuaranteeSection,
    PlantBasedRemediesSection,
    Links,
    FlameleanIngredientsSection,
    NaturalSolutionSection,
    FourStarOfTheShowSection,
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
