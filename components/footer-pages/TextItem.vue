<template>
	<div class="d-flex flex-column align-items-start fs-5 col-xl-9 mx-auto">
		<div v-for="(item, i) in text" :key="i" class="mb-4">
			<div v-html="item"></div>
		</div>
	</div>
</template>

<script>
export default {
	name: "TextItem",
	props: {
		text: {
			type: Array,
			default: [],
		},
	},
};
</script>

<style scoped></style>
