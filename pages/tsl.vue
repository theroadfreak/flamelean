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
    <flamelean-features-section/>
    <plant-based-remedies-section/>
    <pricing-section/>
    <offer-section :bg-color="true"/>
    <pricing-section :user-review="true" :free-shipping-title="true"/>
    <money-back-guarantee-investment-section/>
    <pricing-section :user-review="true" :free-shipping-title="true"/>
    <money-back-guarantee-section/>
    <frequently-asked-questions-section/>
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
import PlantBasedRemediesSection from "@/components/tsl/PlantBasedRemediesSection";
import CommonSideEffectsSection from "~/components/tsl/CommonSideEffectsSection";
import TheMostImportantThingSection from "~/components/tsl/TheMostImportantThingSection";
import MedicationConsequencesSection from "~/components/tsl/MedicationConsequencesSection";
import MoneyBackGuaranteeInvestmentSection from "@/components/tsl/MoneyBackGuaranteeInvestmentSection";
import MoneyBackGuaranteeSection from "@/components/index/MoneyBackGuaranteeSection";
import FlameleanFeaturesSection from "@/components/index/FlameleanFeaturesSection";

export default {
  name: "tsl",
  components: {
    FlameleanFeaturesSection,
    MoneyBackGuaranteeSection,
    MoneyBackGuaranteeInvestmentSection,
    TheMostImportantThingSection,
    MedicationConsequencesSection,
    CommonSideEffectsSection,
    PlantBasedRemediesSection,
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
