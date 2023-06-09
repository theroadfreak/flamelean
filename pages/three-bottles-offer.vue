<template>
	<main>
		<hero-section />
		<product-offer-section :card="card" :link="link" :no="no" />
		<features-section />
		<next-step
			link="https://flamelean.pay.clickbank.net/?cbitems=3bottlesflameleandownsell&cbur=d"
		/>
	</main>
</template>

<script>
import HeroSection from "@/components/three-bottles-offer/HeroSection.vue";
import LastProductOfferSection from "@/components/ProductOfferSection.vue";
import FeaturesSection from "@/components/FeaturesSection";
import NextStep from "@/components/NextStep.vue";
import ProductOfferSection from "@/components/ProductOfferSection";

export default {
	name: "three-bottles-offer",
	layout: "no-navbar",
	components: {ProductOfferSection, NextStep, FeaturesSection, HeroSection},
	data() {
		return {
			title: "3 Bottles Offer | Flamelean",
			card: {
				quantity: 3,
				price: 99,
				img: "three-bottles-offer/flamelean-product.png",
				alt: "Three bottles of Flamelean",
				perDay: 0.81,
				savings: 78,
			},
			link: "https://flamelean.pay.clickbank.net/?cbitems=3bottlesflameleandownsell&cbur=a",
			no: "https://flamelean.pay.clickbank.net/?cbitems=3bottlesflameleandownsell&cbur=d",
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
