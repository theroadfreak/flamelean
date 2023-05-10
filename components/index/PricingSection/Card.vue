<template>
  <div class="zoom cursor-pointer card bg-white py-4"
       :class="[{ 'mt-lg-3' : card.quantity !== 6 },
        { 'border border-4 border-success' : card.quantity === 6 },
        { 'pb-5' : card.initialSumPrice === '' }
        ]">
    <div class="d-flex flex-column align-items-center text-secondary text-center">
      <div class="fs-2 fw-bold mb-1">{{ card.quantity }} {{ card.quantity > 1 ? 'Bottles' : 'Bottle' }}</div>
      <div :class="{ 'mb-3' : card.quantity !== 3 }">{{ card.supplyDays }} Days Supply</div>
      <div class="ratio cst-ratio" :class="{ 'mb-3' : card.quantity !== 3 }">
        <img :src="require('../../../assets/images/index/pricing-section/' + card.image)"
             :alt="card.alt"
             class="object-fit-contain"
        />
      </div>
      <div class="d-flex align-items-start position-relative mb-1" :class="{ 'mb-3' : card.quantity !== 3 }">
        <div class="display-4 fw-bold">
          <span class="me-1">$</span>{{ card.bottlePrice }}
        </div>
        <div class="position-absolute ms-1 mt-1 start-100 top-0">/bottle</div>
      </div>
      <div v-if="card.freeBonuses === true"
           class="rounded rounded-4 bg-success ps-2 pe-5 py-1"
           :class="card.freeShipping === true ? 'mb-2' : 'mb-3'"
      >
        <div class="d-flex align-items-center">
          <img src="../../../assets/images/index/pricing-section/tick.svg"
               alt="Tick icon"
               width="15"
               height="15"
               class="me-2"
          />
          <div class="text-secondary fw-bold small fst-italic">
            2 FREE BONUSES!
          </div>
        </div>
      </div>
      <div v-if="card.freeShipping === true" class="rounded rounded-4 bg-success ps-2 pe-5 py-1 mb-3">
        <div class="d-flex align-items-center">
          <img src="../../../assets/images/index/pricing-section/tick.svg"
               alt="Tick icon"
               width="15"
               height="15"
               class="me-2"
          />
          <div class="text-secondary fw-bold small fst-italic">
            Free US Shipping
          </div>
        </div>
      </div>
      <div class="w-100 px-4 mb-4">
        <button class="btn btn-primary rounded rounded-3 small w-100 text-white py-3 d-flex align-items-center justify-content-center">
          <img src="../../../assets/images/index/pricing-section/shopping-cart-icon.svg"
               alt="Shopping Cart Icon"
               width="30"
               height="26"
               class="me-2"
          />
          <span class="fw-bold">YES! BUY IT NOW</span>
        </button>
      </div>
      <div class="d-flex mb-3">
        <img v-for="paymentCardImage in paymentCardsImages"
             :src="require('../../../assets/images/index/pricing-section/' + paymentCardImage)"
             alt="Payment Card"
             width="40"
             height="26"
             class="me-2"
        />
      </div>
      <div class="d-flex align-items-center text-secondary">
        <span v-if="card.discountedSumPrice" class="fs-3 fw-bold me-3">
          $ {{ card.discountedSumPrice }}
        </span>
        <span v-if="card.initialSumPrice" class="fs-5 text-decoration-line-through text-color-a7a7a7">
          $ {{ card.initialSumPrice }}
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    card: {
      type: Object,
      required: true,
    }
  },
  data() {
    return {
      paymentCardsImages: [
        'visa.svg',
        'mastercard.svg',
        'american-express.svg',
        'discover.svg',
      ]
    }
  }
}
</script>

<style scoped>
.cst-ratio {
  --bs-aspect-ratio: calc(1 / 2 * 100%);
}

.text-color-a7a7a7 {
  color: #a7a7a7;
}
</style>
