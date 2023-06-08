<template>
	<section class="container d-flex flex-column align-items-center py-5">
		<h2 class="text-secondary text-center fw-bold mb-5 line-height-normal">
			Our 4 “Star Of The Show”<br />
			Research-Backed Ingredients:
		</h2>
		<div
			class="row d-flex align-items-start justify-content-center col-xl-10"
		>
			<div
				v-for="(ingredient, i) in ingredients"
				:key="i"
				class="col-11 col-md-6 col-lg-5 mb-4 text-secondary"
				:class="i % 2 !== 0 ? 'offset-lg-1' : ''"
			>
				<div class="d-flex flex-column">
					<div class="ratio ratio-3x2 mb-3">
						<img
							:src="
								require('../../assets/images/tsl/four-star-of-the-show-section/' +
									ingredient.image)
							"
							:alt="ingredient.name + ' ingredient'"
							class="object-fit-contain"
						/>
					</div>
					<div class="fs-5 fw-bold mb-3">{{ ingredient.name }}</div>
					<div
						v-for="paragraph in ingredient.paragraphs"
						class="small"
					>
						<p>{{ paragraph }}</p>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
export default {
	name: "FourStarOfTheShowSection",
	data() {
		return {
			ingredients: [
				{
					image: "magnesium.png",
					name: "Magnesium",
					paragraphs: [
						`A Harvard Medical School study published in Diabetes
             Care found magnesium could improve insulin sensitivity and lower fasting plasma glucose and glucagon levels.`,
						`The study involved 63 participants who received either magnesium supplements or a placebo for 16 weeks.`,
						`Results showed magnesium made significant
             improvements in insulin sensitivity, and fasting plasma glucose levels, as well as a reduction in glucagon levels.`,
					],
				},
				{
					image: "chromium.png",
					name: "Chromium",
					paragraphs: [
						`A trial published in the Journal of Clinical Pharmacy and Therapeutics investigated the effect
            of chromium on fasting plasma glucagon levels. The study involved 40 participants who
            received either chromium or a placebo for 12 weeks.`,
						`Results showed chromium made a significant reduction in fasting plasma glucagon levels compared to
             the placebo group.`,
						`But that’s not all…`,
						`The same study also found chromium significantly reduced fasting plasma glucagon levels.`,
					],
				},
				{
					image: "cinnamon.png",
					name: "Cinnamon",
					paragraphs: [
						`A meta-analysis of 10 trials published in the Journal of Medicinal Food investigated the effect
             of cinnamon on glucose control.`,
						`The study involved 543 participants who received either cinnamon or a placebo for at least 4 weeks.`,
						`Results showed that cinnamon significantly reduced fasting plasma glucose, HbA1c, and plasma
             glucagon levels compared to the placebo group.`,
					],
				},
				{
					image: "gymnema.png",
					name: "Gymnema",
					paragraphs: [
						`A study published in the Journal of Ethnopharmacology investigated the effect of Gymnema on glucose control.`,
						`The study involved 22 participants who received Gymnema or a placebo for 18-20 weeks.`,
						`Results showed the Gymnema made a significant reduction in fasting plasma glucose and glucagon levels
             compared to the placebo group.`,
					],
				},
			],
		};
	},
};
</script>

<style scoped></style>
