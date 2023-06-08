<template>
	<section class="container py-5 text-center">
		<div class="mb-5">
			<flamelean-impact-features
				:features="features"
				title="That’s Right, If You Don’t Think Your New Life Is…"
			/>
		</div>
		<div>
			<h2 class="text-secondary fw-bold mb-5">
				This Really Is A Game-Changer!
			</h2>
			<div
				v-for="text in textParts"
				:key="text"
				class="col-12 d-flex flex-column align-items-center"
			>
				<div
					class="col-12 col-lg-10 col-xl-8 text-secondary mb-1"
					v-html="text"
				></div>
			</div>
		</div>
	</section>
</template>

<script>
import FlameleanImpactFeatures from "@/components/FlameleanImpactFeatures";
export default {
	name: "FlameleanImpactSection",
	components: {FlameleanImpactFeatures},
	data() {
		return {
			textParts: [
				`<span class="fw-bold">Just ONE of those 4 ingredients would support healthy blood glucose levels and trigger
long-lasting weight loss.</span>`,
				"Now picture uniting all of them in scientifically-proven amounts…",
				`And adding 15 other well-researched botanicals, nutrients, and minerals to boost and accelerate
your transformation even more!`,
				`That's precisely what we've created – and it's the reason our customers are looking
and feeling incredible.`,
			],
			features: [
				"Supporting healthy blood sugar levels",
				"A breeze now your body is able to use insulin more effectively, naturally",
				"Joyful because you’re no longer fighting a losing battle against carb and sugar cravings",
				"Energetic now the herbal blend is giving you a natural boost",
				"Super easy to lose weight because you’re fuller for longer and actually enjoy being active",
				"Empowering every time you’re told: “wow, you’ve lost so much weight - you look great!”",
				"The best it’s ever been now you’re finally in control",
			],
		};
	},
};
</script>

<style scoped></style>
