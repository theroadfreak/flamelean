<template>
	<section class="bg-image">
		<div class="container d-flex flex-column justify-content-center py-5">
			<h2 class="text-white text-center fw-bold mb-5">
				That’s Why We Created…
			</h2>
			<div class="row d-flex justify-content-center align-items-center">
				<div class="d-flex justify-content-center col-12 col-lg-6">
					<div class="col-12 col-md-8 col-lg-12 col-xxl-10">
						<div class="ratio ratio-6x5">
							<img
								src="../../assets/images/index/flamelean-carnitine-substance/flamelean.png"
								alt="Flamelean medicine"
								class="object-fit-contain"
							/>
						</div>
					</div>
				</div>
				<div class="col-12 col-lg-6 d-flex flex-column">
					<img
						src="../../assets/images/index/flamelean-carnitine-substance/flamelean-logo.svg"
						alt="Flamelean logo"
						width="230"
						height="50"
						class="mb-5"
					/>
					<p class="col-12 col-xl-10 text-white mb-4">
						FlameLean's unique and proprietary formula is the first
						in the world to combine 19 clinically-researched
						ingredients… That mimics the function of your GLP-1
						hormone… Helping to slow the movement of food through
						your stomach… So you can feel fuller for longer, lose
						weight effortlessly, and most importantly… Regain
						control of your blood sugar levels naturally - without
						stress, worry or fear.
					</p>
					<div class="col-12 col-md-3">
						<nuxt-link
							class="nav-item btn btn-light text-primary rounded rounded-3 px-3 mt-2 mt-lg-0"
							to="/#pricing-section"
						>
							Order Now
						</nuxt-link>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
export default {
	name: "WhyWeCreatedFlameleanSection",
};
</script>

<style scoped>
.bg-image {
	background-image: url("../../assets/images/index/flamelean-carnitine-substance/bg-image.png");
	background-size: cover;
	background-position: top;
}
</style>
