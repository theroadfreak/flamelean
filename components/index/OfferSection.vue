<template>
	<section :class="bgColor ? 'bg-light' : 'bg-image'">
		<div class="container py-5">
			<div class="row">
				<div class="col-12 d-flex justify-content-center text-center">
					<div class="col-11 col-md-7 col-lg-6 col-xxl-4 mb-5">
						<h2
							class="fw-bold line-height-normal mb-0"
							:class="bgColor ? 'text-secondary' : 'text-white'"
						>
							Order
							<span
								:class="
									bgColor ? 'text-primary' : 'text-success'
								"
								>6 Bottles</span
							>
							or
							<span
								:class="
									bgColor ? 'text-primary' : 'text-success'
								"
								>3 Bottles</span
							>
							and Get
							<span
								class="border-bottom border-3"
								:class="
									bgColor
										? 'border-secondary'
										: 'border-success'
								"
							>
								2 FREE Bonuses</span
							>
							!
						</h2>
					</div>
				</div>
				<div class="col-12 mt-md-3">
					<div
						class="row d-flex justify-content-center align-items-stretch"
					>
						<div
							v-for="(bonus, i) in bonuses"
							:key="bonus.bookTitle"
							class="col-11 col-sm-10 col-md-6 col-lg-5 col-xxl-4 d-flex justify-content-center"
							:class="{'mb-5 mb-md-0': i !== bonuses.length - 1}"
						>
							<bonus :bonus="bonus" :bg-color="bgColor" />
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
import Bonus from "@/components/index/OfferSection/Bonus.vue";

export default {
	name: "OfferSection",
	components: {Bonus},
	props: {
		bgColor: {
			type: Boolean,
			default: false,
		},
	},
	data() {
		return {
			bonuses: [
				{
					image: "book-1.png",
					alt: "1 Day Kickstart Detox Book",
					bookTitle: `Why Blood Sugar Level is So Important for Weight Loss`,
					price: "59.95",
					paragraph: `Acetyl-l-carnitine; L-carnitine Carnitine is a
substance that helps the body turn fat into
energy. Your body makes it in the liver and
kidneys and stores it in the skeletal muscles,
heart, brain, and sperm.`,
					number: 1,
				},
				{
					image: "book-2.png",
					alt: "Renew You",
					bookTitle: `EAT TO FIT - 30 Days Meal Plan`,
					price: "49.95",
					paragraph: `Acetyl-l-carnitine; L-carnitine Carnitine is a
substance that helps the body turn fat into
energy. Your body makes it in the liver and
kidneys and stores it in the skeletal muscles,
heart, brain, and sperm.`,
					number: 2,
				},
			],
		};
	},
};
</script>

<style scoped>
.bg-image {
	background-image: url("../../assets/images/index/offer-section/bg-image.png");
	background-size: cover;
	background-position: top;
}
</style>
