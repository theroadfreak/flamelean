<template>
	<section
		class="container d-flex flex-column align-content-center text-center fs-5"
	>
		<div
			v-for="(item, i) in list"
			:key="i"
			class="mb-3 d-flex justify-content-center align-items-center"
		>
			<img
				src="../../../assets/images/tsl/common-side-effects-section/x-icon.svg"
				alt="X icon"
				width="24"
				height="24"
				class="me-2"
			/>
			<span class="text-secondary">{{ item }}</span>
		</div>
	</section>
</template>

<script>
export default {
	name: "TheXedList",
	props: {
		list: {
			type: Array,
			default: null,
		},
	},
};
</script>

<style scoped></style>
