<template>
  <main>
    <flamelean-logo/>
    <shipping-and-returns-section/>
    <custom-footer/>
  </main>
</template>

<script>
import ShippingAndReturnsSection from "@/components/footer-pages/ShippingAndReturnsSection";
import FlameleanLogo from "@/components/footer-pages/FlameleanLogo";
import CustomFooter from "@/components/footer-pages/CustomFooter";
export default {
  name: "shipping-and-returns",
  components: {CustomFooter, FlameleanLogo, ShippingAndReturnsSection},
  layout: 'no-navbar'
}
</script>

<style scoped>

</style>
