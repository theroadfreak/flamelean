<template>
	<main>
		<intro-section />
		<shipping-and-returns-section />
		<custom-footer />
	</main>
</template>

<script>
import ShippingAndReturnsSection from "@/components/footer-pages/ShippingAndReturnsSection";
import CustomFooter from "@/components/footer-pages/CustomFooter";
import IntroSection from "@/components/footer-pages/IntroSection";
export default {
	name: "shipping-and-returns",
	components: {IntroSection, CustomFooter, ShippingAndReturnsSection},
	layout: "no-navbar",
};
</script>

<style scoped></style>
