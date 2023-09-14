<template>
	<main>
		<intro-section />
		<shipping-and-returns-section />
		<CustomFooter />
	</main>
</template>

<script>
import ShippingAndReturnsSection from "@/components/footer-pages/ShippingAndReturnsSection";
import CustomFooter from "@/components/layouts/CustomFooter.vue";
import IntroSection from "@/components/footer-pages/IntroSection";
export default {
	name: "shipping-and-returns",
	components: {IntroSection, ShippingAndReturnsSection, CustomFooter},
	layout: "no-navbar",
};
</script>

<style scoped></style>
