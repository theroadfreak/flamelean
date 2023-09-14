<template>
	<main>
		<intro-section />
		<product-offer-section :card="card" :link="link" :no="no" />
		<features-section />
		<!-- <next-step
			link="TODO: add link"
		/> -->
	</main>
</template>

<script>
import IntroSection from "@/components/six-bottles-offer/IntroSection";
import ProductOfferSection from "@/components/ProductOfferSection";
import FeaturesSection from "@/components/FeaturesSection";
import NextStep from "@/components/NextStep";

export default {
	name: "six-bottles-offer",
	components: {NextStep, FeaturesSection, ProductOfferSection, IntroSection},
	layout: "no-navbar",
	data() {
		return {
			title: "6 Bottles Offer | Flamelean",
			card: {
				quantity: 6,
				price: 199,
				img: "six-bottles-offer/flamelean-product.png",
				alt: "Six bottles of Flamelean",
				perDay: 1.09,
				savings: 155,
			},
			link: "", // TODO: add link
			no: "", // TODO: add link
		};
	},
	head() {
		return {
			title: this.title,
			meta: [
				{
					hid: "og:title",
					property: "og:title",
					content: this.title,
				},
			],
		};
	},
};
</script>

<style scoped></style>
