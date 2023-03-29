<template>
  <section class="container py-5">
    <div class="row d-flex justify-content-center align-items-center align-items-xl-start">
      <div class="order-1 order-md-0 col-12 col-lg-7 mb-md-4 mb-lg-0">
        <div class="text-primary small">January 2023</div>
        <h1 class="fw-bold mb-4 mb-sm-5 text-secondary title-font-size">
          Stanford Scientists Discover A Shocking New Cause of Belly Fat, And it’s Not What You Think...
        </h1>
        <p class="mb-0 text-secondary pe-lg-4">
          Acetyl-l-carnitine; L-carnitine Carnitine is a substance that
          helps the body turn fat into energy. Your body makes it in the
          liver and kidneys and stores it in the skeletal muscles, heart,
          brain, and sperm. Usually, your body can make all the
          carnitine it needs. Some people, however, may not have
          enough carnitine because their bodies cannot make enough
          or cannot transport it into tissues so it can be used. Other
          conditions, such as angina or intermittent claudication, can
          also cause low levels of carnitine in the body, as can some
          medications. Carnitine has been proposed as a treatment
          for many conditions because it acts as an antioxidant.
          Antioxidants fight harmful particles in the body known as
          can some medications.
        </p>
      </div>
      <div class="order-0 order-md-1 col-12 col-lg-5 mb-5 mb-md-0">
        <div class="ratio ratio-2x3 custom-max-height">
          <img src="../../assets/images/index/stanford-scientists-article/scientist.png"
               alt="Scientist"
               class="object-fit-contain custom-max-height"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "StanfordScientistsArticleSection"
}
</script>

<style scoped>
@media (max-width: 991.98px) {
  .custom-max-height {
    max-height: 70vh;
  }
}

.title-font-size {
  font-size: 2.1rem;
}

@media (min-width: 1200px) {
  .custom-max-height {
    max-height: 75vh;
  }

  .title-font-size {
    font-size: 2.3rem;
  }
}

@media (max-width: 767.98px) {
  .title-font-size {
    font-size: 1.8rem;
  }
}
</style>
