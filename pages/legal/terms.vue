<template>
<main>
  <flamelean-logo/>
  <terms-section/>
  <custom-footer/>
</main>
</template>

<script>
import TermsSection from "@/components/legal/TermsSection";
import FlameleanLogo from "@/components/footer-pages/FlameleanLogo";
import CustomFooter from "@/components/footer-pages/CustomFooter";
export default {
  name: "terms",
  layout: 'no-navbar',
  components: {CustomFooter, FlameleanLogo, TermsSection}
}
</script>

<style scoped>

</style>
