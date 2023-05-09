<template>
  <main>
    <flamelean-logo/>
    <privacy-section/>
    <custom-footer/>
  </main>
</template>

<script>
import PrivacySection from "@/components/legal/PrivacySection";
import FlameleanLogo from "@/components/footer-pages/FlameleanLogo";
import CustomFooter from "@/components/footer-pages/CustomFooter";
export default {
  name: "privacy",
  layout: 'no-navbar',
  components: {CustomFooter, FlameleanLogo, PrivacySection}
}
</script>

<style scoped>

</style>
