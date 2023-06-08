<template>
	<section
		class="container d-flex flex-column align-items-center text-center py-5"
	>
		<!-- <as-talked-about-in-section /> -->
	</section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";
// import AsTalkedAboutInSection from "@/components/AsTalkedAboutInSection";

export default {
	name: "Intro",
	components: {/*AsTalkedAboutInSection,*/ TitleSubtitleText},
	data() {
		return {
			texts: [],
		};
	},
};
</script>

<style scoped></style>
