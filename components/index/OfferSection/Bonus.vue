<template>
  <div class="d-flex flex-column w-100 h-100">
    <div class="card bg-white w-100 h-75 mb-4">
      <div class="card-img-top">
        <div class="ratio ratio-1x1">
          <img :src="require('../../../assets/images/index/offer-section/' + bonus.image)"
               :alt="bonus.alt"
               class="object-fit-cover"
          />
        </div>
      </div>
      <div class="card-body d-flex justify-content-center text-center">
        <div class="fs-5 fw-bold text-primary">BONUS #{{ bonus.number }}
          <span class="fw-normal ms-2 text-secondary">{{ bonus.bookTitle }}</span>
        </div>
      </div>
    </div>
    <div class="d-flex flex-column justify-content-center text-start">
      <div class="text-white fs-4 mb-4">RRP:
        <span class="text-decoration-line-through text-decoration-color">{{ bonus.price }}</span>
        <span class="ms-2">Today: <span class="text-success fw-bold">FREE</span></span>
      </div>
      <div class="fs-6 text-white line-height-normal">
        {{ bonus.paragraph }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Bonus",
  props: {
    bonus: {
      type: Object,
      required: true,
    }
  }
}
</script>

<style scoped>
.text-decoration-color {
  text-decoration-color: #16FF3B !important;
}
</style>
