<template>
	<section class="container pt-5 pb-3 justify-content-center">
		<h1 class="fw-bold text-center mb-4">Anti-Spam Policy</h1>

		<text-item :text="text" />

		<CustomFooter />
	</section>
</template>

<script>
import TextItem from "../footer-pages/TextItem.vue";
import CustomFooter from "../layouts/CustomFooter.vue";

export default {
	name: "AntiSpamSection",
	components: {
		TextItem,
		CustomFooter,
	},
	data() {
		return {
			text: [
				"In order to serve our customers, we collect personally identifiable information, like names, addresses, phone numbers, email addresses, IP addresses, any notes or testimonials or comments that you provide to us or on our websites, and sometimes credit card information when such information is voluntarily submitted by our visitors.",
				"We will only use your personal information for the following purposes:",
				"To operate, improve, or promote our services; to provide customer service or support; to market our products and services through email marketing, SMS marketing; advertising – including retargeting via Google, Facebook, and similar companies; and notifications; to perform accounting, administrative, and legal tasks; to process payments; to help prevent fraud, to help diagnose problems with our servers and software, to gather broad demographic information, and to offer you products and services; to deliver the products and/or services to you that you have requested; to validate your compliance with the terms and conditions; for content improvement and feedback purposes; to contact you, when necessary, regarding your use of the Website or product(s); for the few situations described below to better serve you.",
				"We will NEVER share your personally identifiable information with third parties unless you have given us explicit permission to do so, such as in order to fulfill a third party offer that you have accepted from us. By permitting us to collect this information, you will be able to receive information on other products and services that may be of interest to you, including related third-party offers that we may send to you. You also enable us to personalize your experience with us so that we can provide you with the highest quality of service.",
				"By submitting your email address on this Website, you agree to receive email from Us. You can cancel your participation in any of these email lists at any time by clicking the opt-out link or other unsubscribe option that is included in each respective email. We only send emails to people who have authorized us to contact them, and purchased products from us, either directly, or through a third party. We do not send unsolicited commercial emails, because we hate spam as much as you do.",
			],
		};
	},
};
</script>
