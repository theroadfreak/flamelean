<template>
  <div>
    <!-- ClickBank Trust Badge -->
    <script src='//cbtb.clickbank.net/?vendor=flamelean'></script>
    <intro-section/>
    <nuxt/>
    <pricing-section :user-review="true" :free-shipping-title="true"/>
    <money-back-guarantee-section/>
    <custom-footer/>
  </div>
</template>

<script>
import PricingSection from "@/components/index/PricingSection";
import MoneyBackGuaranteeSection from "@/components/index/MoneyBackGuaranteeSection";
import CustomFooter from "@/components/layouts/CustomFooter";
import IntroSection from "@/components/footer-pages/IntroSection";


export default {
  name: "footer-pages-layout",
  components: {IntroSection, CustomFooter, MoneyBackGuaranteeSection, PricingSection}
}
</script>

<style scoped>

</style>
