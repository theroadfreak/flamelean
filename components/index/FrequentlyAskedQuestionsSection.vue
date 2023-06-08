<template>
	<section>
		<div class="container d-flex flex-column align-items-center py-5">
			<h2 class="fw-bold text-center text-secondary mb-5">
				Frequently Asked Questions
			</h2>
			<div class="col-11 col-sm-12 col-lg-11 col-xl-10">
				<div
					class="accordion accordion-flush bg-transparent w-100"
					id="accordionFAQ"
				>
					<div
						v-for="(accordionItem, i) in accordionItems"
						class="accordion-item w-100 rounded rounded-3 bg-e6e6e6"
						:class="{'mb-3': i !== accordionItems.length - 1}"
					>
						<h2 class="accordion-header" :id="'heading_' + i">
							<button
								class="accordion-button rounded bg-e6e6e6 border border-0 collapsed text-secondary"
								type="button"
								data-bs-toggle="collapse"
								:data-bs-target="'#collapse_' + i"
								aria-expanded="false"
								:aria-controls="'#collapse_' + i"
							>
								<span class="py-1">{{
									accordionItem.question
								}}</span>
							</button>
						</h2>
						<div
							:id="'collapse_' + i"
							class="accordion-collapse rounded-bottom bg-e6e6e6 collapse"
							:aria-labelledby="'heading_' + i"
							data-bs-parent="#accordionFAQ"
						>
							<div
								v-if="accordionItem.answer !== ''"
								class="accordion-body small text-secondary col-12 col-lg-11 col-xl-10 pt-0 pb-4"
								v-html="accordionItem.answer"
							></div>
							<div
								v-if="accordionItem.img"
								class="accordion-body text-secondary col-12 col-sm-8 col-lg-6 pt-0 pb-4"
							>
								<div class="ratio ratio-1x1">
									<img
										:src="
											require('../../assets/images/index/faq-section/' +
												accordionItem.img)
										"
										:alt="accordionItem.alt"
										class="object-fit-contain object-position-left"
									/>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
export default {
	name: "FrequentlyAskedQuestionsSection",
	data() {
		return {
			accordionItems: [
				{
					question: "Who is FlameLean for?",
					answer: `FlameLean is for anyone who wants to maintain healthy blood glucose levels<br/>
           Plus, it’s for anyone who wants to feel fuller for longer, crave sweet and salty foods less,
           and have a supportive boost with losing weight.`,
				},
				{
					question:
						"What makes FlameLean different to anything else I’ve tried?",
					answer: `No other natural health supplement mimics the hormone GLP-1 to create a 3-step approach to good health:
          <ol>
          <li>Moving sugar out of your blood and into other body tissues to be used for energy instead of stored as fat</li>
          <li>Slowing the movement of food through the stomach to decrease appetite and lose weight</li>
          </ol>
          This is the only natural health supplement that contains 19 unique botanicals, herbs, minerals
          and vitamins that can help boost insulin sensitivity and maintain blood glucose control.`,
				},
				{
					question: "How do I take FlameLean?",
					answer: `Easy! Just take one capsule with your favourite beverage every day.<br/>
          We recommend taking it with a meal, in the morning, as it can help give you energy for the rest of your day.`,
				},
				{
					question: "What is the full ingredients list?",
					answer: ``,
					img: "ingredients-list.png",
					alt: "Full ingredients list",
				},
				{
					question: "What if it does not work for me?",
					answer: `We’re so confident in FlameLean that we’re backing your order with our no questions asked 180-day
           “empty bottle” guarantee.<br/>
           Try it for 6 months and if you’re not happy, or if you change your mind for
           any reason at all, simply contact our friendly customer support team
           (details provided with your order).`,
				},
				{
					question:
						"When will I receive my order and do I have to pay shipping?",
					answer: `As soon as you place your order it will be shipped same day and arrive at your door within 5-7
          business days.<br/>
          The best part is, when you order 3 or 6 bottles you don’t pay a shipping or handling fee!`,
				},
			],
		};
	},
};
</script>

<style scoped>
.bg-e6e6e6 {
	background-color: #e6e6e6;
}
</style>
