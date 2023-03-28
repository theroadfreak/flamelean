<template>
  <section class="bg-image">
    <div class="container py-5">
      <div class="row d-flex justify-content-center align-items-center">
        <div class="d-flex justify-content-center col-12 col-lg-6">
          <div class="col-12 col-md-10 col-lg-12 col-xxl-10">
            <div class="ratio ratio-6x5">
              <img src="../../assets/images/index/flamelean-carnitine-substance/flamelean.png"
                   alt="Flamelean medicine"
                   class="object-fit-contain"
              />
            </div>
          </div>
        </div>
        <div class="col-12 col-lg-6 d-flex flex-column">
          <img src="../../assets/images/index/flamelean-carnitine-substance/flamelean-logo.svg"
               alt="Flamelean logo"
               width="230"
               height="50"
               class="mb-5"
          />
          <p class="col-12 col-xl-10 text-white mb-5 paragraph-font-size">
            Acetyl-l-carnitine; L-carnitine Carnitine is a substance that
            helps the body turn fat into energy. Your body makes it in the
            liver and kidneys and stores it in the skeletal muscles, heart,
            brain, and sperm. Usually, your body can make all the
            carnitine it needs. Some people, however, may not have enough carnitine because their bodies cannot
            make enough or cannot transport it into tissues so it can be
            used. Other conditions, such as angina or intermittent
            claudication, can also cause low levels of carnitine in the
            body, as can some medications. Carnitine has been
            proposed as a treatment.
          </p>
          <div>
            <button class="btn bg-white text-primary rounded rounded-3 py-2 px-4">Order Now</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "FlameleanCarnitineSubstanceSection"
}
</script>

<style scoped>
.bg-image {
  background-image: url("../../assets/images/index/flamelean-carnitine-substance/bg-image.png");
  background-size: cover;
  background-position: top;
}

.paragraph-font-size {
  font-size: 1.1rem;
}

@media (max-width: 767.98px) {
  .paragraph-font-size {
    font-size: 1rem;
  }
}
</style>
