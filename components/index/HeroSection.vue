<template>
  <section class="bg-image">
    <div class="container py-5">
      <div class="row d-flex align-items-center justify-content-center">
        <div class="col-12 col-md-6 mb-4 mb-md-0">
          <div class="ratio ratio-16x9">
            <img src="../../assets/images/index/hero-section/hero-img.png"
                 alt="Flamelean Product"
                 class="object-fit-contain"
            />
          </div>
        </div>
        <div
          class="col-12 col-md-6 d-flex flex-column align-items-center align-items-md-start text-center text-md-start">
          <div class="text-primary small">Manufactured in USA</div>
          <h1 class="display-5 fw-bold mb-5 text-secondary">Lose weight <span class="fw-normal">with</span> Flamelean
          </h1>
          <ul class="list-unstyled">
            <li v-for="feature in features" :key="feature" class="d-flex align-items-center mb-3">
              <img src="../../assets/images/index/check.svg"
                   alt="Check icon"
                   width="17" height="17"
                   class="me-2"
              />
              <span class="text-secondary">{{ feature }}</span>
            </li>
          </ul>
          <button class="btn btn-primary text-white rounded rounded-3 py-2 px-5">Order Now</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HeroSection",
  data() {
    return {
      features: [
        'Miracle Appetite Suppressant',
        'Fat Blocker',
        'Fastest Weight Loss',
      ],
    }
  }
}
</script>

<style scoped>
.bg-image {
  background-image: url("../../assets/images/index/hero-section/bg-image.png");
  background-size: cover;
  background-position: top;
}
</style>
