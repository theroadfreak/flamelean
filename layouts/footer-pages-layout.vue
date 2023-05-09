<template>
  <div>
    <flamelean-logo/>
    <nuxt/>
    <pricing-section :user-review="true" :free-shipping-title="true"/>
    <money-back-guarantee-section/>
    <custom-footer/>
  </div>
</template>

<script>
import FlameleanLogo from "@/components/footer-pages/FlameleanLogo";
import PricingSection from "@/components/index/PricingSection";
import MoneyBackGuaranteeSection from "@/components/index/MoneyBackGuaranteeSection";
import CustomFooter from "@/components/layouts/CustomFooter";


export default {
  name: "footer-pages-layout",
  components: {CustomFooter, MoneyBackGuaranteeSection, PricingSection, FlameleanLogo}
}
</script>

<style scoped>

</style>
