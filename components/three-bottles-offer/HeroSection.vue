<template>
	<section class="bg-primary">
		<div class="container pt-3">
			<img
				src="../../assets/images/layouts/logo.svg"
				alt="Flamelean's Logo"
				width="150"
				height="34"
			/>
		</div>
		<div
			class="container d-flex flex-column align-items-center text-center pt-5 pb-2"
		>
			<h1>
				<span class="d-block text-success fw-bold mb-3"
					>Congratulations, you’ve been selected!!</span
				>
				<span class="text-white">Claim Your $78 Instant Discount</span>
			</h1>
		</div>
	</section>
</template>

<script>
import ProgressBar from "@/components/ProgressBar.vue";

export default {
	name: "HeroSection",
	components: {ProgressBar},
};
</script>

<style scoped></style>
