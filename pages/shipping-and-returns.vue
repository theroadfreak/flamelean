<template>
  <main>
    <flamelean-new-logo/>
    <shipping-and-returns-section/>
    <custom-footer-pages/>
  </main>
</template>

<script>
import FlameleanNewLogo from "@/components/no-layout-footer-pages/FlameleanNewLogo";
import ShippingAndReturnsSection from "@/components/no-layout-footer-pages/ShippingAndReturnsSection";
import CustomFooterPages from "@/components/no-layout-footer-pages/CustomFooterPages";
export default {
  name: "shipping-and-returns",
  components: {CustomFooterPages, ShippingAndReturnsSection, FlameleanNewLogo},
  layout: 'no-navbar'
}
</script>

<style scoped>

</style>
