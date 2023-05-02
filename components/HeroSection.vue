<template>
  <section class="bg-image">
    <div class="container py-5">
      <div class="row d-flex align-items-center justify-content-center">
        <div class="col-12 col-md-9 col-lg-8 col-xl-6 mb-4 mb-md-0">
          <div class="ratio ratio-16x9">
            <img src="../assets/images/index/hero-section/hero-img.png"
                 alt="Flamelean Product"
                 class="object-fit-contain"
            />
          </div>
        </div>
        <div
          class="col-12 col-lg-11 col-xl-6 d-flex flex-column align-items-center align-items-xl-start text-center text-xl-start">
          <div class="text-primary small">Manufactured in USA</div>
          <h1 class="display-6 fw-bold mb-4 text-secondary">
            Hollywood’s New Weight
            Loss Secret Revealed: The
            Hype, Hazard & Better
            Alternative
          </h1>
          <div class="text-secondary">
            <div class="mb-3">
              Have you noticed that in the last year all your favorite celebrities are appearing skinnier
              than they ever have before?
            </div>
            <div class="mb-3">
              Doctors all over the world are all talking about it…
            </div>
            <div class="mb-2">
              Read More:
            </div>
            <div class="mb-5 mb-xl-4">
              <a
                href="https://www.nbcnews.com/health/health-news/people-diabetes-struggle-find-ozempic-soars-popularity-weight-loss-aid-rcna64916"
                target="_blank"
              >
                https://www.nbcnews.com/health/health-news/people-diabetes-struggle-find-ozempic-soars-popularity-weight-loss-aid-rcna64916
              </a>
            </div>
            <div>
              <img src="../assets/images/index/hero-section/features.svg"
                   alt="Flamelean Features Icons"
                   width="300"
                   height="54"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HeroSection",
}
</script>

<style scoped>
.bg-image {
  background-image: url("../assets/images/index/hero-section/bg-image.png");
  background-size: cover;
  background-position: top;
}
</style>
