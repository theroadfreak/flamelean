<template>
  <section class="bg-primary">
    <div class="container d-flex flex-column align-items-center py-5">
      <div
        class="col-12 col-lg-10 card d-flex flex-column align-items-center text-center py-5 px-4 bg-white rounded rounded-3">
        <div class="mb-4 text-black">
          <div>On this private page only…</div>
          <div>You can stock up on FlameLean by adding</div>
        </div>
        <div class="text-black mb-2">
          <span class="fs-3 fw-bold text-uppercase">{{ card.quantity }} Bottles </span>
          <span class="fs-4">to your order for just</span>
        </div>
        <div class="display-4 text-secondary fw-bold mb-2 d-flex flex-column justify-content-center">
          <span>${{ card.price }}</span>
        </div>
        <div class="col-12 mb-3 text-danger display-5 fw-light">{{ formattedCountdown }}</div>
        <div class="col-12 col-sm-10 col-lg-9 col-xl-8 mb-4">
          <div class="ratio ratio-21x9">
            <img :src="require('../assets/images/' + card.img)"
                 :alt="card.alt"
                 class="object-fit-contain"
            />
          </div>
        </div>
        <div class="col-12 col-md-9 border-top border-2 border-light mb-4"></div>
        <div class="text-black mb-4 d-flex flex-column align-items-center">
          <span>That’s just ${{ card.perDay }} per day.</span>
          <span class="small text-4D4D4D pt-3"><i>*You won't be billed monthly</i></span>
        </div>
        <div class="col-12 col-md-9 border-top border-2 border-light"></div>
        <div class="text-black my-3">
          It’s also a savings of ${{ card.savings }}<br/>
          off the regular retail price of FlameLean
        </div>
        <div class="col-12 col-md-9 py-4 mb-4 mb-md-5 bg-success text-secondary">
          Plus FREE shipping to your door
        </div>
        <div class="col-11 col-md-7 col-lg-6 d-flex text-center justify-content-center">
          <button
            class="zoom cursor-pointer w-100 btn btn-primary text-white py-3 rounded rounded-3 d-flex align-items-center justify-content-center text-center">
            <span class="fw-bold ">
              <img src="../assets/images/shopping-cart-icon.svg"
                   width="30"
                   height="26"
                   alt="Shopping Cart icon"
                   class="me-2"
              />
              YES, UPGRADE MY ORDER!</span>
          </button>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "ProductOfferSection",
  props: {
    card: {
      type: Object,
      required: true,
    }
  },
  data() {
    return {
      countdown: 300,
      countdownInterval: null
    }
  },
  mounted() {
    this.startCountdown()
  },
  methods: {
    startCountdown() {
      this.countdownInterval = setInterval(() => {
        if (this.countdown > 0) {
          this.countdown--;
        } else
          clearInterval(this.countdownInterval);
      }, 1000)
    }
  },
  computed: {
    formattedCountdown() {
      const hours = Math.floor(this.countdown / 3600);
      const minutes = Math.floor((this.countdown % 3600) / 60);
      const seconds = this.countdown % 60;
      const formattedHours = hours.toString().padStart(2, '0');
      return `${formattedHours}:${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;
    }
  },
}
</script>

<style scoped>
</style>
