<template>
	<main>
		<intro-section />
		<ClientOnly>
			<terms-section />
		</ClientOnly>
		<!-- <custom-footer /> -->
		<CustomFooter />
	</main>
</template>

<script>
import TermsSection from "@/components/legal/TermsSection";
import CustomFooter from "@/components/layouts/CustomFooter.vue";
import IntroSection from "@/components/footer-pages/IntroSection";
export default {
	name: "terms",
	layout: "no-navbar",
	components: {IntroSection, TermsSection, CustomFooter},
};
</script>

<style scoped></style>
