<template>
	<section class="bg-image">
		<div class="container py-5 d-flex flex-column align-items-center">
			<h2
				v-if="freeShippingTitle"
				class="text-white text-center fw-bold mb-5"
			>
				Every 3 And 6-Bottle Order Gets Free Shipping Too!
			</h2>
			<div class="col-12">
				<div class="row d-flex justify-content-center">
					<div
						v-for="(card, i) in cards"
						:key="card.bottlePrice"
						class="col-10 col-sm-8 col-md-6 col-lg-4 col-xl-3"
						:class="{
							'mb-4 mb-lg-0 me-md-1 me-lg-0':
								i !== cards.length - 1,
						}"
					>
						<card :card="card" />
					</div>
				</div>
			</div>
			<div
				v-if="userReview"
				class="small text-white text-center mt-5 col-12 col-md-9 col-lg-6 col-xl-5"
			>
				"My clothes fit so much better and more comfortably. I’ve lost
				52 pounds since starting.” Stacey Bollinger, Maryland
			</div>
		</div>
	</section>
</template>

<script>
import Card from "@/components/index/PricingSection/Card.vue";

export default {
	name: "PricingSection",
	components: {Card},
	props: {
		userReview: {
			type: Boolean,
			default: false,
		},
		stockAvailableText: {
			type: Boolean,
			default: false,
		},
		freeShippingTitle: {
			type: Boolean,
			default: false,
		},
	},
	data() {
		return {
			cards: [
				{
					quantity: 1,
					supplyDays: 30,
					image: "flamelean-bottle.png",
					alt: "Flamelean Bottle",
					bottlePrice: 59,
					initialSumPrice: "",
					discountedSumPrice: "",
					freeBonuses: false,
					freeShipping: false,
					link: "https://flamelean.pay.clickbank.net/?cbitems=1bottleflamelean",
				},
				{
					quantity: 6,
					supplyDays: 120,
					image: "flamelean-6-bottles.png",
					alt: "Flamelean 6 Bottles",
					bottlePrice: 39,
					initialSumPrice: 354,
					discountedSumPrice: 234,
					freeBonuses: true,
					freeShipping: true,
					withClickIcon: true,
					link: "https://flamelean.pay.clickbank.net/?cbitems=6bottlesflamelean",
				},
				{
					quantity: 3,
					supplyDays: 90,
					image: "flamelean-3-bottles.png",
					alt: "Flamelean 3 Bottles",
					bottlePrice: 49,
					initialSumPrice: 177,
					discountedSumPrice: 147,
					freeBonuses: true,
					freeShipping: true,
					link: "https://flamelean.pay.clickbank.net/?cbitems=3bottlesflamelean",
				},
			],
		};
	},
};
</script>

<style scoped>
.bg-image {
	background-image: url("../../assets/images/index/pricing-section/bg-image.svg");
	background-size: cover;
	background-position: top;
}
</style>
