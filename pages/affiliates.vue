<template>
	<section id="affiliates" class="bg-image">
		<div class="container">
			<div class="row mb-5">
				<h1 class="text-center fw-bold">
					Promote <span class="text-primary">Flamelean</span> Now
					<br />
					Get <span class="text-primary">75% Per Sale</span>
				</h1>
			</div>

			<div class="bg-primary rounded p-3 mb-4 shadow-sm">
				<div class="d-flex justify-content-between">
					<div class="row">
						<img
							src="@/assets/images/index/hero-section/hero-img.png"
							alt="Flamelean Product"
							class="object-fit-contain"
							width="250"
						/>
					</div>
					<div class="row">
						<p class="text-white fw-bold display-6 mb-4">
							Flamelean™ is available to promote easily and
							quickly on the BuyGoods affiliate network.
						</p>
						<p class="text-white fs-4">
							They track all your clicks and conversion and send
							out your payments
							<span class="text-decoration-underline"
								>every week</span
							>! Creating an account is
							<span class="text-decoration-underline">FREE</span>.
							Follow the steps below to get started:
						</p>
					</div>
				</div>
			</div>

			<!-- Tracking pixels start -->
			<div
				id="tracking__pixels"
				class="bg-primary rounded shadow-sm mb-4 p-3"
			>
				<div id="trackingpixles__title" class="mb-4">
					<h1 class="text-center text-white fw-bold">
						Tracking Pixels
					</h1>
				</div>

				<div id="trackingpixles__content">
					<p class="text-white fs-4">
						BuyGoods allows you to place all your tracking pixels
						(such as Facebook, Yahoo, Google, Voluum and more) right
						from you BuyGoods account.
					</p>
				</div>
			</div>
			<!-- Tracking pixels end -->

			<!-- Email Swipes Start -->
			<div
				class="container bg-white rounded shadow-sm mb-4 p-3"
				id="email__Swipes"
			>
				<div id="main__text">
					<h1 class="text-center fw-bold">Email Swipes</h1>
				</div>
				<div id="secondary__text">
					<h3 class="text-center">
						Use these email swipes to promote Flamelean to your
						email list.
					</h3>

					<div class="accordion" id="accordionEmailSwipes">
						<div
							class="accordion-item"
							v-for="i in listOfItems"
							:key="i.id"
						>
							<h2 class="accordion-header">
								<button
									class="accordion-button collapsed"
									type="button"
									data-bs-toggle="collapse"
									:data-bs-target="'#' + i.id"
									aria-expanded="false"
									:aria-controls="i.id"
								>
									{{ i.title }}
								</button>
							</h2>
							<div
								:id="i.id"
								class="accordion-collapse collapse"
								:aria-labelledby="i.id"
								data-bs-parent="#accordionEmailSwipes"
							>
								<div class="accordion-body">
									<h4>Subject Lines:</h4>
									<ol style="list-style: lower-alpha">
										<li v-for="line in i.subjectLines">
											{{ line }}
										</li>
									</ol>
									<p v-for="p in i.paragraphs" v-html="p"></p>
									<img
										v-if="i.picture"
										:src="
											require(`@/assets/images/` +
												i.picture)
										"
										:width="i.width"
										alt="picture"
										class="object-fit-contain"
									/>
									<p
										v-for="p in i.restOfParagraphs"
										v-html="p"
									></p>
								</div>
							</div>
						</div>
					</div>

					<!-- <div v-for="i in listOfItems" class="swiper-slide">
      <div class="slider-content">
        <h3>{{ i.title }}</h3>
        <h4>Subject Lines:</h4>
        <ol style="list-style: lower-alpha">
          <li v-for="line in i.subjectLines">{{ line }}</li>
        </ol>
        <p v-for="p in i.paragraphs" v-html="p"></p>
        <img
          v-if="i.picture"
          :src="require(`@/assets/images/` + i.picture)"
          :width="i.width"
          alt="picture"
          class="object-fit-contain"
        />
        <p v-for="p in i.restOfParagraphs" v-html="p"></p>
      </div>
    </div> -->
				</div>
			</div>
			<!-- Email Swipes End -->

			<!-- Demographics start -->
			<div id="demographics" class="bg-white rounded shadow-sm p-3 mb-4">
				<div id="demographics__title">
					<h1 class="text-center fw-bold">Demographics</h1>
				</div>

				<div id="demographics__content" class="container">
					<div class="row">
						<div class="col me-2">
							<div
								class="row mb-2 bg-black rounded bg-opacity-10 text-center"
							>
								<h1 class="text-primary fw-bold">Age</h1>
								<span class="fs-4">40 - 85</span>
							</div>
							<div
								class="row mb-2 bg-black rounded bg-opacity-10 text-center"
							>
								<h1 class="text-primary fw-bold">Gender</h1>
								<p>
									Primary
									<span class="text-decoration-underline"
										>female</span
									>, secondary
									<span class="text-decoration-underline"
										>male</span
									>
									also converts very well.
								</p>
							</div>
							<div
								class="row bg-black rounded bg-opacity-10 text-center"
							>
								<h1 class="text-primary fw-bold">Location</h1>
								<p>
									Primary
									<span class="text-decoration-underline"
										>USA</span
									>, secondary UK, Canada, Australia, New
									Zealand.
								</p>
							</div>
						</div>
						<div
							class="col d-flex flex-column justify-content-center"
						>
							<div
								class="row mb-2 bg-black rounded bg-opacity-10 text-center"
							>
								<h1 class="text-primary fw-bold">Device</h1>
								<p>
									Primary
									<span class="text-decoration-underline"
										>mobile</span
									>, secondary
									<span class="text-decoration-underline"
										>tablet</span
									>, tertiary desktop.
									<br />
									<span class="fw-bold">Note:</span> Our
									website is optimized for maximum conversions
									on all devices!
								</p>
							</div>
							<div
								class="row bg-black rounded bg-opacity-10 text-center"
							>
								<h1 class="text-primary fw-bold">
									Traffic Types
								</h1>
								<p>
									We convert and have affiliates successfully
									making industry-leading ROIs all traffic
									types such as Facebook, Email, Native,
									YouTube, TikTok and more!
								</p>
							</div>
						</div>
					</div>
				</div>
			</div>
			<!-- Demographics end -->

			<!-- Images start -->
			<div id="images" class="bg-white rounded shadow-sm p-3 mb-4">
				<div id="images__title">
					<h1 class="text-center fw-bold">Images</h1>
				</div>

				<p class="fs-4">
					You are permitted to use the following imagery in your
					promotions. You are not allowed to use any imagery found on
					this website aside from that detailed below. Click to open
					the image in a new window then right-click
					<span class="fw-bold">"Save Image As"</span> to save to your
					computer.
				</p>

				<div id="images__content">
					<div id="content__title">
						<h1 class="text-center text-primary fw-bold">
							Product Images
						</h1>
					</div>

					<div class="container text-center">
						<div class="row mb-2">
							<div
								class="col me-2 border border-5 rounded border-primary"
							>
								<img
									src="@/assets/images/index/pricing-section/flamelean-bottle.png"
									alt="Flamelean Product"
									class="object-fit-contain"
									width="250"
									height="225"
								/>
							</div>
							<div
								class="col me-2 border-5 rounded border border-primary"
							>
								<img
									src="@/assets/images/index/pricing-section/flamelean-3-bottles.png"
									alt="Flamelean Product"
									class="object-fit-contain"
									width="250"
								/>
							</div>
							<div
								class="col me-2 border-5 rounded border border-primary"
							>
								<img
									src="@/assets/images/index/pricing-section/flamelean-6-bottles.png"
									alt="Flamelean Product"
									class="object-fit-contain"
									width="250"
								/>
							</div>
						</div>
						<div class="row">
							<div
								class="col me-2 border-5 rounded border border-primary"
							>
								<img
									src="@/assets/images/index/offer-section/book-1.png"
									alt="Flamelean Product"
									class="object-fit-contain"
									width="250"
									height="225"
								/>
							</div>
							<div
								class="col me-2 border-5 rounded border border-primary"
							>
								<img
									src="@/assets/images/index/offer-section/book-2.png"
									alt="Flamelean Product"
									class="object-fit-contain"
									width="250"
									height="225"
								/>
							</div>
							<div
								class="col border border-5 rounded border-primary"
							>
								<img
									src="@/assets/images/index/flamelean-carnitine-substance/flamelean.png"
									alt="Flamelean Product"
									class="object-fit-contain"
									width="250"
									height="225"
								/>
							</div>
						</div>
					</div>
				</div>
			</div>
			<!-- Images end -->

			<!-- Contact us start -->
			<div id="contact" class="bg-white rounded shadow-sm p-3 mb-4">
				<div id="contact__title">
					<h1 class="text-center fw-bold">Contact us</h1>
				</div>

				<div id="contact__content" class="container">
					<p class="fs-4">
						If you need anything else, email your dedicated
						affiliate manager at
						<span class="fw-bold">support@flamelean.com</span> and
						they will assist you as soon as possible. We look
						forward to working with you.
					</p>
				</div>
			</div>
			<!-- Contact us end -->

			<!-- Affiliate terms start -->
			<div id="affiliate_terms" class="text-black p-3">
				<div id="affiliate_terms__title">
					<h1 class="text-center fw-bold">Affiliate Terms</h1>
				</div>

				<div id="content">
					<span class="">
						By promoting Flamelean, you hereby agree to the
						following terms of service. If an affiliate breaches the
						following terms they will be instantly
						banned/blacklisted from promoting our products, and any
						future sales will be voided without warning.
						<br />
						<ol>
							<li>
								Affiliates
								<span class="text-decoration-underline"
									>may NOT</span
								>
								copy, transcribe, paraphrase, reproduce or
								otherwise use in any format any video or part of
								video found on this website in their promotions.
							</li>
							<li>
								Affiliates
								<span class="text-decoration-underline"
									>may NOT</span
								>
								use any before or after photos found on this
								website or found within this website's video
								content in their promotions.
							</li>
							<li>
								Affiliates
								<span class="text-decoration-underline"
									>may NOT</span
								>
								bid on keywords (word, sentence or phrase) on
								any search engine such as Google, Bing and Yahoo
								where any part of the keyword targeted contains
								the word "Flamelean" such as "buy Flamelean",
								"Flamelean reviews" etc.
							</li>
							<li>
								Affiliates
								<span class="text-decoration-underline"
									>may NOT</span
								>
								falsely represent themselves as the creators or
								owners of Flamelean in their promotions.
							</li>
							<li>
								Affiliates
								<span class="text-decoration-underline"
									>may NOT</span
								>
								use words such as "fraud", "scam" or similar
								terminology in their promotions including but
								not limited to, Ad content, landing pages, video
								titles, written content or other metadata.
							</li>
							<li>
								Affiliates
								<span class="text-decoration-underline"
									>may NOT</span
								>
								promote, sell, wholesale or resell Flamelean on
								any retail site including but not limited to
								Amazon, eBay and Google Store.
							</li>
							<li>
								Affiliates
								<span class="text-decoration-underline"
									>may NOT</span
								>
								direct prospects directly to the checkout page
								bypassing the Flamelean website. All customers
								must purchase through the Flamelean website.
							</li>
							<li>
								Affiliates understand Flamelean is solely
								responsible for customer service.
							</li>
							<li>
								Affiliates' websites, promotions and material
								(regardless of country of domicile)
								<span class="text-decoration-underline"
									>MUST</span
								>
								be in compliance with all applicable laws,
								regulations, and guidelines, including without
								limitation the Federal Trade Commission Act
								("FTC Act"), the Controlling the Assault of
								Non-Solicited Pornography and Marketing Act of
								2003 ("CAN-SPAM Act"), Federal Trade Commission
								("FTC") regulations and guidelines implementing
								the FTC Act and the CAN-SPAM Act, the FTC's
								Guides Concerning the Use of Endorsements and
								Testimonials in Advertising ("FTC Testimonials
								Guide"), the National Advertising Division
								decisions of the Better Business Bureau, and
								other federal and state consumer protection
								laws, regulations, and guidelines.
							</li>
						</ol>
						<br />
						This bonus offer has been created by the applicable
						Seller and not by BuyGoods. Accordingly, BuyGoods is not
						responsible for any information contained in the offer,
						including, but not limited to, any product information,
						promotions, incentives, expected returns or other
						information contained herein. In addition, BuyGoods is
						not responsible for any links to third party websites in
						conjunction with this offer. Such links do not imply any
						endorsement by BuyGoods of such websites or the content,
						products or services available from such websites. By
						clicking on or accessing a third party website listed,
						you acknowledge sole responsibility for and assume all
						risk arising from your use of any such websites.
					</span>
				</div>
			</div>
			<!-- Affiliate terms end -->
		</div>
	</section>
</template>

<script>
export default {
	name: "affiliates",
	data() {
		return {
			listOfItems: [
				{
					id: 1,
					title: "Email Swipe 1 - Science Mech Tease",
					subjectLines: [
						"Do THIS to burn fat in the morning",
						"Jessica lost 40 lbs in 2 months WITHOUT surgery",
						"Harvard: diabetics should try THIS for weight loss",
					],
					paragraphs: [
						"Harvard Medical School is proving a macronutrient has dramatic effects on diabetics…",
						"Improving insulin sensitivity and helping you feel fuller for longer.",
						"In fact, Jessica tried it and lost 40 lbs of weight in 2 just months!",
						"Not only was she forced to buy a whole new wardrobe…",
						"But Jessica finally felt in control of her blood sugar levels…",
						"The natural way and with zero stress.",
						"<span class='text-primary text-decoration-underline'> >> Try THIS Harvard-approved macronutrient today << </span>",
					],
				},
				{
					id: 2,
					title: "Email Swipe 2 - Celebrity Gossip",
					subjectLines: [
						"Kim Kardadshian before and after (pics inside)",
						"Kim Kardashian’s dieting secret",
						"REVEALED: Kim Kardashian weight loss truth",
					],
					paragraphs: [
						"I just read a post on Kim Kardashian…",
						"About how she really lost 16 pounds in 3 weeks.",
						"Take a look:",
					],
					picture:
						"tsl/the-biggest-suspect-section/kim-kardashian-transformation.png",
					width: 500,
					restOfParagraphs: [
						"Rumors are circulating Hollywood right now…",
						"That Kim and other A-List celebrities (Rebel Wilson, Elon Musk and more)...",
						"Are using a diabetes medication to slim down effortlessly.",
						"Here’s the thing…",
						"The medication they’re injecting themselves with costs an eye watering $1,300 per month.",
						"Plus, it comes with a boxed warning…",
						"The strongest safety-related warning required by the FDA!",
						"The good news is…",
						"There’s a more natural, safer, cheaper alternative to this medication.",
						"It works the same way by:",
						"Using that sugar for energy instead of storing it as stubborn fat…",
						"Decreasing your appetite and helping you lose weight effortlessly",
						"So, if you have trouble losing weight and managing your blood sugar levels…",
						"The easiest thing you can do is…",
						"=> Try THIS natural, safe, affordable alternative every morning",
						"It’s going to give your body everything it needs to start burning fat again…",
						"And manage your blood glucose without the stress.",
						"Stay healthy!",
					],
				},
				{
					id: 3,
					title: "Email Swipe 3 - Shorter Celeb Gossip",
					subjectLines: [
						"lose 40 pounds in 2 months like Kim Kardashian",
						"Try Kim Kardashian’s weight loss 'secret'",
						"lose weight FASTER than Kim Kardashian (safely)",
					],
					paragraphs: [
						"Have you noticed celebrities getting skinnier than ever before",
					],
					picture: "affliate/affliate1.png",
					width: 300,
					restOfParagraphs: [
						"It’s got nothing to do with a new workout routine, diet, or surgery procedure.",
						"It’s a lot more simple than that.",
						"You see, it’s been rumored the Kardashian’s are taking diabetes medication…",
						"That comes at an eye-watering price.",
						"$1,300 fee per month to be exact.",
						"And it’s not for the faint-hearted.",
						"It has to be injected once weekly in either the thigh, stomach, or upper arm.",
						"Luckily, there’s a more natural, cheaper, invasion-free alternative.",
						"Jessica tried it and lost 40 pounds in just 2 months.",
						"I was shocked when I saw her drop from 210 to 170 pounds!",
						"I practically begged for her secret.",
						"And she generously revealed everything you need to know, here…",
						"<span class='text-primary text-decoration-underline'> => lose 40 pounds in 2 months like Kim Kardashian </span>",
						"<span class='text-primary text-decoration-underline'> => Try Kim Kardashian’s weight loss “secret” </span>",
						"<span class='text-primary text-decoration-underline'> => lose weight FASTER than Kim Kardashian (safely) </span>",
					],
				},
				{
					id: 4,
					title: "Email Swipe 4 - Problem / Solution",
					subjectLines: [
						"THIS is why you can’t lose weight",
						"TRUTH about diabetes and weight loss",
						"losing weight is easy once you know THIS",
						"Rebel Wilson before and after (pics inside)",
					],
					paragraphs: [
						"It’s got nothing to do with a new workout routine, diet, or surgery procedure.",
						"Want to know why you find it so hard to lose weight?",
						"Well, if you have diabetes there’s a very simple reason that not many people talk about.",
						"You see, my friend Jessica has suffered from Type 2 diabetes for over 9 years.",
						"She piled on 40 pounds in the space of 6 months…",
						"And was struggling to lose it ever since.",
						"So, when she saw A-List celebs like Kim Kardashian, Elon Musk, and Rebel Wilson suddenly drop weight in the blink of an eye…",
						"She demanded to know their secret.",
					],
					picture: "affliate/affliate1.png",
					width: 300,
					restOfParagraphs: [
						"Not only did she discover some of them were taking a diabetes medication (and forcing it to sellout nationwide)...",
						"But she uncovered exactly WHY it works so well at helping you lose weight.",
						"Regardless of whether you’re obese, have diabetes, or are perfectly healthy.",
						"You see, it has everything to do with a hormone inside of you that…",
						"When switched “off” can cause you to always feel hungry…",
						"Crave sweet and sugary foods…",
						"And hold onto fat for dear life.",
						"Making it near impossible to shift.",
						"But the beauty of this hormone is that, once it’s switched “on”…",
						"The reverse happens.",
						"Jesscia was able to lose 40 pounds in the space of 2 months!",
						"WITHOUT injecting herself with needles, or asking for prescriptions like the celebs.",
						"<span class='text-primary text-decoration-underline'> => You can read Jessica’s full story here</span>",
						"If you’ve been trying to lose weight for a long time, or gain control of your fluctuating blood sugar levels…",
						"Then I encourage you to click the link now while her site’s still online.",
						"Big pharma is trying frantically to take it down…",
						"Because she’s sharing a more natural alternative than what they have to offer you.",
						"Stay healthy!",
					],
				},
			],
		};
	},
};
</script>

<style scoped>
.bg-image {
	background-image: url("../assets/images/index/hero-section/bg-image.png");
	background-size: cover;
	background-position: top;
}
</style>
