<template>
	<div class="d-flex flex-column text-secondary">
		<div class="d-flex mb-2">
			<img
				v-for="i in 5"
				src="../../../assets/images/index/reviews-section/star.svg"
				width="25"
				height="25"
				class="me-1"
			/>
		</div>
		<div class="fs-5 fw-bold mb-2">{{ review.title }}</div>
		<p class="mb-0">{{ review.paragraph }}</p>
	</div>
</template>

<script>
export default {
	name: "Review",
	props: {
		review: {
			type: Object,
			required: true,
		},
	},
};
</script>

<style scoped></style>
