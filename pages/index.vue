<template>
	<main>
		<hero-section />
		<the-blood-sugar-secret-section />
		<!-- <as-talked-about-in-section/> -->
		<pricing-section />
		<flamelean-ingredients-section id="ingredients" />
		<flamelean-features-section />
		<offer-section />
		<shipping-section />
		<flamelean-impact-section id="flamelean-impact-section" />
		<pricing-section id="pricing-section" />
		<frequently-asked-questions-section id="faq" />
	</main>
</template>

<script>
import HeroSection from "@/components/HeroSection.vue";
import FlameleanIngredientsSection from "@/components/FlameleanIngredientsSection.vue";
import FlameleanFeaturesSection from "@/components/index/FlameleanFeaturesSection.vue";
import OfferSection from "@/components/index/OfferSection.vue";
import ShippingSection from "@/components/index/ShippingSection.vue";
import ReviewsSection from "@/components/index/ReviewsSection.vue";
import PricingSection from "@/components/index/PricingSection.vue";
import FrequentlyAskedQuestionsSection from "@/components/index/FrequentlyAskedQuestionsSection.vue";
import TheBloodSugarSecretSection from "@/components/index/TheBloodSugarSecretSection.vue";
import FlameleanImpactSection from "@/components/index/FlameleanImpactSection.vue";
// import AsTalkedAboutInSection from "@/components/AsTalkedAboutInSection";

export default {
	name: "index",
	components: {
		// AsTalkedAboutInSection,
		FlameleanImpactSection,
		TheBloodSugarSecretSection,
		FrequentlyAskedQuestionsSection,
		PricingSection,
		ReviewsSection,
		ShippingSection,
		OfferSection,
		FlameleanFeaturesSection,
		FlameleanIngredientsSection,
		HeroSection,
	},
	data() {
		return {
			title: "Flamelean",
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
