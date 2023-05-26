<template>
  <main>
    <intro-section />
    <privacy-section />
    <custom-footer />
  </main>
</template>

<script>
import PrivacySection from "@/components/legal/PrivacySection";
import CustomFooter from "@/components/footer-pages/CustomFooter";
import IntroSection from "@/components/footer-pages/IntroSection";
export default {
  name: "privacy",
  layout: "no-navbar",
  components: { IntroSection, CustomFooter, PrivacySection },
};
</script>

<style scoped></style>
