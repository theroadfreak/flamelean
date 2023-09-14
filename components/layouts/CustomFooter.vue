<template>
	<div class="bg-primary text-white">
		<footer-links class="bg-secondary" :footer-links="links.slice(0, 6)" />
		<footer-links :footer-links="links.slice(7, links.length)" />
	</div>
</template>

<script>
import FooterLinks from "@/components/layouts/CustomFooter/FooterLinks";

export default {
	name: "CustomFooter",
	components: {FooterLinks},
	data() {
		return {
			links: [
				{
					name: "Home",
					link: "/",
				},
				{
					name: "Benefits",
					link: "/footer-linked-pages/benefits",
				},
				{
					name: "Customer Reviews",
					link: "/footer-linked-pages/customer-reviews",
				},
				{
					name: "Ingredients",
					link: "/footer-linked-pages/ingredients",
				},
				{
					name: "Label",
					link: "/footer-linked-pages/flamelean-label",
				},
				{
					name: "Side Effect",
					link: "/footer-linked-pages/side-effects",
				},
				{
					name: "Home",
					link: "/",
				},
				{
					name: "Product Support",
					href: "mailto:support@flamelean.com",
				},
				{
					name: "Order Support",
					href: "https://www.buygoods.com/",
				},
				{
					name: "Terms",
					link: "/legal/terms",
				},
				{
					name: "Privacy",
					link: "/legal/privacy",
				},
				{
					name: "Shipping",
					link: "/footer-linked-pages/shipping-and-returns",
				},
			],
			text: ``,
		};
	},
};
</script>

<style scoped></style>
