<template>
  <section class="container pt-5 pb-3 justify-content-center">
    <h1 class="fw-bold text-center mb-4">Shipping And Returns</h1>
    <text-item :text="text.slice(0,1)"/>
    <product-and-order-support/>
    <h2 class="fw-bold text-center mb-4">Shipping</h2>
    <text-item :text="text.slice(1,3)"/>
    <div class="d-flex flex-column align-items-start fs-5 col-lg-9 mx-auto mb-2">
      <div><b>Average Shipping Times:</b></div>
      <div><b>US/Canada:</b> 5-7 business days.</div>
      <div><b>International</b> 10-16 business days</div>
    </div>
    <h2 class="fw-bold text-center mb-4">Returns</h2>
    <text-item :text="text.slice(3,7)"/>
    <div class="d-flex flex-column align-items-start fs-5 col-lg-9 mx-auto mb-3">
      <div>FlameLean</div>
      <div>9655 E 35th Drive. Suite 100</div>
      <div>Aurora, CO 80011</div>
    </div>
    <text-item :text="text.slice(7,9)"/>
    <product-and-order-support/>
  </section>
</template>

<script>
import TextItem from "@/components/no-layout-footer-pages/TextItem";
import ProductAndOrderSupport from "@/components/no-layout-footer-pages/ProductAndOrderSupport";
export default {
  name: "ShippingAndReturnsSection",
  components: {ProductAndOrderSupport, TextItem},
  data() {
    return{
      text: [
        'Please note: Your order was processed by our merchant ClickBank. It will be ClickBank that shows up on your credit card or billing statement! If you are not the cardholder, inform them of this! If you purchased any upgrades, they will show up as separate transactions.',
        'We offer shipping to most countries around the world. We will aim to ship out your order same day. Otherwise it will be shipped out next day. We ship orders out 7 days a week, excluding all recognized days of US holidays and postal holidays.',
        'You will receive a shipping notification along with your tracking link to locate and track the status of your order in transit when your item has shipped. Any questions regarding your tracking or shipment please contact us using the information below.',
        'In order to obtain a full refund for an order you must return all bottles of the order you wish to be refunded, be they empty, full or partially full back to our fulfillment center at the address listed below, within sixty (60) days since the order date. If the entirety of the order is not received and processed by the fulfillment center within 60 days after the order date, we will not issue your refund. In this event any goods received will not be returned to you.',
        'Along with your returned order you must clearly include details regarding your order, including (1) Your ClickBank Order ID (found in your order receipt), (2) Your Full Name, (3) Your Full Address where the shipment was received, (4) Your Email Address and (5) your Phone Number so that a member of our fulfillment center staff can clearly read and process your return. Contact our support team at support@flamelean.com if you need help retrieving this information.',
        'Failure to fully meet both refund requirements A) and B) above will result in our inability to refund you. The customer must pay for the shipping to return the products to us. Once our fulfillment center has received your order and processed the information, you will be issued a refund. Your refund will be credited back to your bank account and may take up to 5-10 business days to show in your statement, depending on the speed of the processing bank.',
        `<b>Physical Returns Address</b>`,
        'Please note: due to the costs involved in shipping orders for international delivery we currently do not refund shipping fees for orders that are delivered outside of the US. We will continue to refund the cost of the bottles you have ordered as per our policy above. For international orders you may be liable to pay customs charges and these would be non-refundable.',
        'Also note: due to the costs involved in shipping orders for international delivery, for any initial purchase of Alpilean to be delivered outside of the US, free shipping promotions do not apply. Free shipping promotions will still apply for any upgrades made where applicable, regardless of delivery location.'
      ]
    }
  }
}
</script>

<style scoped>

</style>
