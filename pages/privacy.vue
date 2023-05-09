<template>
  <main>
    <flamelean-new-logo/>
    <privacy-section/>
    <custom-footer-pages/>
  </main>
</template>

<script>
import FlameleanNewLogo from "@/components/no-layout-footer-pages/FlameleanNewLogo";
import PrivacySection from "@/components/no-layout-footer-pages/PrivacySection";
import CustomFooterPages from "@/components/no-layout-footer-pages/CustomFooterPages";
export default {
  name: "privacy",
  layout: 'no-navbar',
  components: {CustomFooterPages, PrivacySection, FlameleanNewLogo}
}
</script>

<style scoped>

</style>
