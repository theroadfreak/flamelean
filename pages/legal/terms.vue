<template>
	<main>
		<intro-section />
		<terms-section />
		<custom-footer />
	</main>
</template>

<script>
import TermsSection from "@/components/legal/TermsSection";
import CustomFooter from "@/components/footer-pages/CustomFooter";
import IntroSection from "@/components/footer-pages/IntroSection";
export default {
	name: "terms",
	layout: "no-navbar",
	components: {IntroSection, CustomFooter, TermsSection},
};
</script>

<style scoped></style>
