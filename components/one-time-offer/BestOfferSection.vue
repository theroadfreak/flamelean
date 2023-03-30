<template>
  <section class="bg-color-e6e6e6">
    <div class="container d-flex flex-column align-items-center py-5">
      <div
        class="col-12 col-xl-10 card d-flex flex-column align-items-center text-center py-5 bg-white rounded rounded-3">
        <div class="fs-4 mb-4">
          +6 Flamelean Bottles For Only
          <span class="text-primary fw-bold">$211.99</span>
        </div>
        <h2 class="text-primary fw-bold mb-2 mb-md-3">
          WORTH: <span class="text-decoration-line-through ms-1">$704</span>
        </h2>
        <h2 class="mb-2 col-11 col-md-12">
          SAVE <span class="text-primary fw-bold">70% OFF + FREE SHIPPING</span>
        </h2>
        <div class="col-10 col-sm-8 col-md-6 col-lg-4 col-xxl-3">
          <div class="ratio ratio-3x2">
            <img src="../../assets/images/one-time-offer/flamelean-product.png"
                 alt="Flamelean product"
                 class="object-fit-contain"
            />
          </div>
        </div>
        <div class="d-flex mb-4">
          <div v-for="(item, i) in time" class="d-flex flex-column align-items-center"
               :class="{ 'me-4' : i !== time.length - 1 }">
            <div class="text-color-eb001b display-6">
              {{ item.value }}
            </div>
            <div class="text-color-4d4d4d text-uppercase">
              {{ item.unit }}
            </div>
          </div>
        </div>
        <div class="col-11 col-sm-10 col-md-9 col-lg-6 d-flex text-center justify-content-center mb-4">
          <button class="w-100 btn btn-primary text-white py-2 custom-line-height rounded rounded-3">
            <span class="fw-bold custom-font-size-sm-screen">Yes! Add This Amazing Offer For $124.99</span><br/>
            <span class="font-size-10px">Limited Time Offer - You will never see this page again.</span>
          </button>
        </div>
        <p class="col-11 col-xxl-10 mb-4 custom-paragraph-font-size text-color-4d4d4d">
          You understand that you will receive (3) extra pouches of Patriot Detox in your package for just $124.99 by
          clicking the
          orange button above. Your bonus pouches will be shipped along with your previous order of Patriot Detox.
        </p>
        <div class="text-primary custom-paragraph-font-size">
          No Thanks, I don't need this now
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BestOfferSection",
  data() {
    return {
      time: [
        {
          value: '01',
          unit: 'hour'
        },
        {
          value: '32',
          unit: 'minute'
        },
        {
          value: '16',
          unit: 'second'
        },
      ]
    }
  }
}
</script>

<style scoped>
.bg-color-e6e6e6 {
  background-color: #E6E6E6;
}

.text-color-eb001b {
  color: #EB001B;
}

.text-color-4d4d4d {
  color: #4D4D4D;
}

.font-size-10px {
  font-size: 10px;
}

.custom-paragraph-font-size {
  font-size: 14px;
}

.custom-line-height {
  line-height: 1.2rem;
}

@media (max-width: 575.98px) {
  .custom-font-size-sm-screen {
    font-size: 0.8rem;
  }
}

@media (max-width: 768px) {
  .custom-paragraph-font-size {
    font-size: 12px;
  }
}
</style>
