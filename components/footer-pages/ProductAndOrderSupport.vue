<template>
	<div>
		<text-item :text="text" />
	</div>
</template>

<script>
import TextItem from "@/components/footer-pages/TextItem";

export default {
	name: "ProductAndOrderSupport",
	components: {TextItem},
	data() {
		return {
			text: [
				`For product support, email us at <a href="mailto:support@flamelean.com">support@flamelean.com.`,
			],
		};
	},
};
</script>

<style scoped></style>
