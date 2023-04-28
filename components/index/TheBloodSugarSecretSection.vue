<template>
  <section class="container py-5">
    <div class="row d-flex justify-content-center align-items-center mb-4 mb-md-5">
      <div class="order-1 order-md-0 col-12 col-lg-7 col-xl-6 col-xxl-5 mb-md-4 mb-lg-0">
        <div class="text-primary small">January 2023</div>
        <h2 class="fw-bold mb-4 mb-sm-5 text-secondary col-lg-10">
          The Blood Sugar Secret That’s Become A Viral Weight Loss Hit
        </h2>
        <div class="text-secondary d-flex flex-column line-height-normal pe-lg-5">
          <span class="mb-4">Have you noticed that in the last year all your favorite celebrities
            are appearing skinnier than they ever have before?</span>
          <span class="mb-4">Doctors all over the world are all talking about it…</span>
          <span class="mb-md-4 mb-lg-0">
            Because they’re deeply concerned.<br/>
And you should be too.<br/>
You see, celebrities like Elon Musk are abusing a prescription
medication…<br/>
Typically formulated for people with Type 2 diabetes, like me
and maybe you.<br/>
But, these celebrities don’t have erratic blood sugar spikes…
And, they’re not at risk of having heart failure or their leg
amputated like us.<br/>
Instead, they’re stocking up on the severely limited drug…
Just so they can lose weight.
          </span>
        </div>
      </div>
      <div class="order-0 order-md-1 col-12 col-lg-5 col-xl-4 mb-5 mb-md-0">
        <div class="ratio ratio-2x3 custom-max-height">
          <img src="../../assets/images/index/the-blood-sugar-secret-section/scientist.png"
               alt="Scientist"
               class="object-fit-contain custom-max-height"
          />
        </div>
      </div>
    </div>
    <div class="d-flex flex-column align-items-center">
      <h2 class="fw-bold text-secondary my-5">
        As Talked About In.
      </h2>
      <div class="col-11 col-md-12 col-xl-11 row d-flex align-items-center justify-content-center">
        <div v-for="(logo, i) in logos" :key="i"
             class="col-6 col-sm-4 col-lg d-flex align-items-center justify-content-center mb-4">
          <img
            :src="require('../../assets/images/index/the-blood-sugar-secret-section/logos/' + logo.image)"
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
  name: "TheBloodSugarSecretSection",
  data() {
    return {
      logos: [
        {
          image: 'forbes.svg',
          alt: 'Forbes logo'
        },
        {
          image: 'new-york-times.svg',
          alt: 'The New York Times logo'
        },
        {
          image: 'vice.svg',
          alt: 'Vice logo'
        },
        {
          image: 'variety.svg',
          alt: 'Variety logo'
        },
        {
          image: 'cbc-news.svg',
          alt: 'CBC News logo'
        },
        {
          image: 'buzz-feed.svg',
          alt: 'BuzzFeed logo'
        },
      ]
    }
  }
}
</script>

<style scoped>
@media (max-width: 575.98px) {
  .custom-max-width {
    max-width: 70%;
  }
}

@media (max-width: 991.98px) {
  .custom-max-height {
    max-height: 70vh;
  }

  .custom-max-width {
    max-width: 90%;
  }
}
</style>
