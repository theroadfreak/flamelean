<template>
<main>
  <flamelean-new-logo/>
  <terms-section/>
  <custom-footer-pages/>
</main>
</template>

<script>
import TermsSection from "@/components/no-layout-footer-pages/TermsSection";
import FlameleanNewLogo from "@/components/no-layout-footer-pages/FlameleanNewLogo";
import CustomFooterPages from "@/components/no-layout-footer-pages/CustomFooterPages";
export default {
  name: "terms",
  layout: 'no-navbar',
  components: {CustomFooterPages, FlameleanNewLogo, TermsSection}
}
</script>

<style scoped>

</style>
