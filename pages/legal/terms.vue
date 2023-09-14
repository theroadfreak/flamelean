<template>
	<main>
		<intro-section />
		<ClientOnly>
			<terms-section />
		</ClientOnly>
		<!-- <custom-footer /> -->
	</main>
</template>

<script>
import TermsSection from "@/components/legal/TermsSection";
// import CustomFooter from "@/components/footer-pages/CustomFooter";
import IntroSection from "@/components/footer-pages/IntroSection";
export default {
	name: "terms",
	layout: "no-navbar",
	components: {IntroSection, TermsSection},
};
</script>

<style scoped></style>
