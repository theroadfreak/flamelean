<template>
  <div>
    <text-item :text="text"/>
  </div>
</template>

<script>

import TextItem from "@/components/no-layout-footer-pages/TextItem";
export default {
  name: "ProductAndOrderSupport",
  components: {TextItem},
  data() {
    return{
      text:[
          `For product support, email us at <a href="support@flamelean.com">support@flamelean.com.`,
          `For order support, visit <a href="https://www.clkbank.com">https://www.clkbank.com</a> or phone ClickBank's Customer Support team at 1-800-390-6035 from the US or +1-208-345-4245 from other countries.`,
      ]
    }
  }
}
</script>

<style scoped>

</style>
