<template>
  <div class="bg-primary text-white">
    <footer-navbar :nav-items="topNavItems"/>
    <div class="p-4 small">
      {{ text }}
    </div>
    <footer-navbar :nav-items="bottomNavItems"/>
  </div>
</template>

<script>
import FooterNavbar from "@/components/layouts/CustomFooter/FooterNavbar";
export default {
  name: "CustomFooter",
  components: {FooterNavbar},
  data() {
    return {
      topNavItems: [
        'Home',
        'Benefits',
        'Customer',
        'Reviews',
        'Ingredients',
        'Label',
        'Side Effect'
      ],
      text: `Statements found on this website have not been evaluated by the Food and Drug Administration.
       Products on this website are not intended to diagnose, treat, cure, or prevent any disease.
       If you are pregnant, nursing, taking medication, or have a medical condition, consult your physician before
       using our products. ClickBank is the retailer of products on this site. CLICKBANK® is a registered trademark
       of Click Sales, Inc., a Delaware corporation located at 1444 S. Entertainment Ave., Suite 410 Boise, ID 83709,
       USA and used by permission. ClickBank's role as retailer does not constitute an endorsement, approval or review
       of these products or any claim, statement or opinion used in promotion of these products.
`,
      bottomNavItems: [
        'Home',
        'Product Support',
        'Order Support',
        'Terms',
        'Privacy',
        'Shipping'
      ]
    }
  }
}
</script>

<style scoped>

</style>
