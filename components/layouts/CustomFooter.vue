<template>
  <div class="bg-primary text-white">
    <footer-links class="bg-secondary" :footer-links="links.slice(0, 6)" />
    <div class="container pt-4">
      <div class="small" style="text-align: justify-all !important">
        {{ text }}
      </div>
    </div>
    <footer-links :footer-links="links.slice(7, links.length)" />
  </div>
</template>

<script>
import FooterLinks from "@/components/layouts/CustomFooter/FooterLinks";

export default {
  name: "CustomFooter",
  components: { FooterLinks },
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
          href: "https://www.clkbank.com/",
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
      text: `Statements found on this website have not been evaluated by the Food and Drug Administration.
       Products on this website are not intended to diagnose, treat, cure, or prevent any disease.
       If you are pregnant, nursing, taking medication, or have a medical condition, consult your physician before
       using our products. ClickBank is the retailer of products on this site. CLICKBANK® is a registered trademark
       of Click Sales, Inc., a Delaware corporation located at 1444 S. Entertainment Ave., Suite 410 Boise, ID 83709,
       USA and used by permission. ClickBank's role as retailer does not constitute an endorsement, approval or review
       of these products or any claim, statement or opinion used in promotion of these products.
       Testimonials, case studies, and examples found on this page are results that have been forwarded to us by users of
       FLAMELEAN products and related products are not intended to represent or guarantee that anyone will achieve the same or similar results.`,
    };
  },
};
</script>

<style scoped></style>
