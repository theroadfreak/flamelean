<template>
	<div>
		<custom-navbar />
		<nuxt />
		<scientific-references-section />
		<custom-footer />
	</div>
</template>

<script>
import CustomNavbar from "../components/layouts/CustomNavbar";
import CustomFooter from "@/components/layouts/CustomFooter";
import ScientificReferencesSection from "@/components/index/ScientificReferencesSection";

export default {
	name: "Default",
	components: {ScientificReferencesSection, CustomFooter, CustomNavbar},
};
</script>

<style scoped></style>
