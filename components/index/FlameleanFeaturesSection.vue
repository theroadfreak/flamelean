<template>
	<section class="background-color-e4dee9">
		<div class="container py-5">
			<div class="row">
				<div class="col-12 d-flex justify-content-center mb-5">
					<img
						src="../../assets/images/index/flamelean-features/flamelean.svg"
						width="230"
						height="50"
						alt="Flamelean"
					/>
				</div>
				<div class="col-12">
					<div class="row d-flex justify-content-center">
						<div
							class="d-none d-lg-flex col-4 d-flex justify-content-center"
							v-for="(features, i) in featuresSlices"
							:key="'large' + i"
						>
							<feature :features="features" />
						</div>
						<div
							class="d-none d-sm-flex d-lg-none col-6 d-flex justify-content-center"
							v-for="(features, i) in featuresSlicesSmScreen"
							:key="'sm' + i"
						>
							<feature :features="features" />
						</div>
						<div
							class="d-flex d-sm-none col-12 justify-content-center"
						>
							<feature :features="features" />
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
import Feature from "@/components/index/FlameleanFeatures/Feature.vue";

export default {
	name: "FlameleanFeaturesSection",
	components: {Feature},
	data() {
		return {
			features: [
				"Natural Formula",
				"Plant Ingredients",
				"Non-GMO",
				"Easy to Swallow",
				"No Stimulants",
			],
		};
	},
	computed: {
		featuresSlices() {
			return this.features.reduce((slices, _, i) => {
				if (i % 2 === 0) {
					slices.push(this.features.slice(i, i + 2));
				}
				return slices;
			}, []);
		},
		featuresSlicesSmScreen() {
			return this.features.reduce((slices, _, i) => {
				if (i % 3 === 0) {
					slices.push(this.features.slice(i, i + 3));
				}
				return slices;
			}, []);
		},
	},
};
</script>

<style scoped>
.background-color-e4dee9 {
	background-color: #e4dee9;
}
</style>
