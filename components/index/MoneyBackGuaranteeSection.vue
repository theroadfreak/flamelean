<template>
  <section class="container d-flex flex-column align-items-center text-center py-5">
    <img src="../../assets/images/index/money-back-guarantee-section/money-back-guarantee-icon.svg"
         alt="Money Back Guarantee Icon"
         width="186"
         height="180"
         class="custom-dimensions-sm-screen mb-4"
    />
    <h1 class="custom-title-size text-primary fw-bold mb-4">
      100% SATISFACTION <br/>
      60-DAY MONEY BACK GUARANTEE
    </h1>
    <p class="mb-4 text-secondary col-12 col-lg-11 col-xl-9">
      We promise your money back if the item you received is not as described, or if your item is not delivered within
      the Buyer Protection period. You can get a refund 15 days after the claim process finishes. This is in
      addition to and does not limit your statutory rights as a consumer, as granted by all mandatory
      laws and regulations applicable in your country of residence.
    </p>
    <div class="col-12 col-lg-9 col-xl-7">
      <div class="ratio ratio-83x15">
        <img src="../../assets/images/index/money-back-guarantee-section/icons.svg"
             alt="Icons"
             class="object-fit-contain"
        />
      </div>
    </div>

  </section>
</template>

<script>
export default {
  name: "MoneyBackGuaranteeSection"
}
</script>

<style scoped>
@media (max-width: 768px) {
  .custom-title-size {
    font-size: 1.8rem !important;
  }
  .custom-dimensions-sm-screen {
    width: 150px !important;
    height: 144px !important;
  }
}
</style>
