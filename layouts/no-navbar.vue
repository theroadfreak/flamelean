<template>
	<div>
		<!-- ClickBank Trust Badge -->
		<script src="https://cbtb.clickbank.net/?vendor=flamelean"></script>
		<nuxt />
		<div
			class="small bg-primary text-white p-3"
			style="text-align: justify-all !important"
		>
			{{ text }}
		</div>
	</div>
</template>

<script>
export default {
	name: "no-navbar",
	data() {
		return {
			text: `Statements found on this website have not been evaluated by the Food and Drug Administration.
       Products on this website are not intended to diagnose, treat, cure, or prevent any disease.
       If you are pregnant, nursing, taking medication, or have a medical condition, consult your physician before
       using our products. ClickBank is the retailer of products on this site. CLICKBANK® is a registered trademark
       of Click Sales, Inc., a Delaware corporation located at 1444 S. Entertainment Ave., Suite 410 Boise, ID 83709,
       USA and used by permission. ClickBank's role as retailer does not constitute an endorsement, approval or review
       of these products or any claim, statement or opinion used in promotion of these products.`,
		};
	},
};
</script>

<style scoped></style>
