<template>
  <section class="container py-5">
    <div class="d-flex flex-column align-items-center">
      <h2 class="fw-bold text-secondary mb-5">As Talked About In.</h2>
      <div
        class="col-11 col-md-12 col-xl-11 row d-flex align-items-center justify-content-center"
      >
        <div
          v-for="(logo, i) in logos"
          :key="i"
          class="col-6 col-sm-4 col-lg d-flex align-items-center justify-content-center mb-4 mb-lg-0"
        >
          <img
            :src="
              require('../assets/images/index/the-blood-sugar-secret-section/logos/' +
                logo.image)
            "
            :alt="logo.alt"
            class="custom-max-width"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AsTalkedAboutInSection",
  data() {
    return {
      logos: [
        {
          image: "forbes.svg",
          alt: "Forbes logo",
        },
        {
          image: "new-york-times.svg",
          alt: "The New York Times logo",
        },
        {
          image: "vice.svg",
          alt: "Vice logo",
        },
        {
          image: "variety.svg",
          alt: "Variety logo",
        },
        {
          image: "cbc-news.svg",
          alt: "CBC News logo",
        },
        {
          image: "buzz-feed.svg",
          alt: "BuzzFeed logo",
        },
      ],
    };
  },
};
</script>

<style scoped>
@media (max-width: 575.98px) {
  .custom-max-width {
    max-width: 70%;
  }
}

@media (max-width: 991.98px) {
  .custom-max-width {
    max-width: 90%;
  }
}
</style>
