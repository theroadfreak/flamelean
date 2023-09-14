<template>
	<div>
		<nuxt />
		<!-- <div
			class="small bg-primary text-white p-3"
			style="text-align: justify-all !important"
		>
			{{ text }}
		</div> -->
	</div>
</template>

<script>
export default {
	name: "no-navbar",
	data() {
		return {
			text: ``,
		};
	},
};
</script>

<style scoped></style>
