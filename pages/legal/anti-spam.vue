<template>
	<main>
		<intro-section />
		<anti-spam-section />
	</main>
</template>

<script>
import IntroSection from "@/components/footer-pages/IntroSection";
import AntiSpamSection from "../../components/legal/AntiSpamSection.vue";
export default {
	name: "privacy",
	layout: "no-navbar",
	components: {IntroSection, AntiSpamSection},
};
</script>
