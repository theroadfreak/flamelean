<template>
	<div class="d-flex flex-column w-100 h-100">
		<div class="card bg-white w-100 h-100 mb-4">
			<div class="card-img-top p-1">
				<div class="ratio ratio-6x7">
					<img
						:src="
							require('../../../assets/images/index/offer-section/' +
								bonus.image)
						"
						:alt="bonus.alt"
						class="object-fit-cover rounded rounded"
					/>
				</div>
			</div>
			<div class="card-body d-flex justify-content-center text-center">
				<div class="fs-5 fw-bold text-primary">
					BONUS #{{ bonus.number }}
					<span class="fw-normal ms-2 text-secondary">{{
						bonus.bookTitle
					}}</span>
				</div>
			</div>
		</div>
		<div class="d-flex flex-column justify-content-center text-start">
			<div
				class="fs-4"
				:class="bgColor ? 'text-secondary' : 'text-white'"
			>
				RRP:
				<span
					class="text-decoration-line-through"
					:class="
						bgColor
							? 'text-primary text-decoration-color-primary'
							: 'text-white text-decoration-color-success'
					"
					>${{ bonus.price }}</span
				>
				<span class="ms-2">
					Today:
					<span
						class="fw-bold"
						:class="bgColor ? 'text-primary' : 'text-success'"
						>FREE</span
					></span
				>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "Bonus",
	props: {
		bonus: {
			type: Object,
			required: true,
		},
		bgColor: {
			type: Boolean,
			default: false,
		},
	},
};
</script>

<style scoped>
.text-decoration-color-success {
	text-decoration-color: #16ff3b !important;
}

.text-decoration-color-primary {
	text-decoration-color: #3c096c !important;
}
</style>
