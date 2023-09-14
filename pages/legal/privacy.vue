<template>
	<main>
		<intro-section />
		<privacy-section />
		<!-- <custom-footer /> -->
		<CustomFooter />
	</main>
</template>

<script>
import PrivacySection from "@/components/legal/PrivacySection";
import CustomFooter from "@/components/layouts/CustomFooter.vue";
import IntroSection from "@/components/footer-pages/IntroSection";
export default {
	name: "privacy",
	layout: "no-navbar",
	components: {IntroSection, CustomFooter, PrivacySection},
};
</script>

<style scoped></style>
