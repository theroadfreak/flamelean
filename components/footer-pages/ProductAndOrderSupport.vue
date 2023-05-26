<template>
  <div>
    <text-item :text="text" />
  </div>
</template>

<script>
import TextItem from "@/components/footer-pages/TextItem";

export default {
  name: "ProductAndOrderSupport",
  components: { TextItem },
  data() {
    return {
      text: [
        `For product support, email us at <a href="mailto:support@flamelean.com">support@flamelean.com.`,
        `For order support, visit <a href="https://www.clkbank.com">https://www.clkbank.com</a>
 or phone ClickBank's Customer Support team at
 <a href="tel:1-800-390-6035" class="fw-bold text-decoration-none">1-800-390-6035</a>
  from the US or
  <a href="tel:+1-208-345-4245" class="fw-bold text-decoration-none">+1-208-345-4245</a>
   from other countries.`,
      ],
    };
  },
};
</script>

<style scoped></style>
