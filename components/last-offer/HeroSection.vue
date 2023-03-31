<template>
  <section class="bg-primary">
    <div class="container pt-3">
      <img
        src="../../assets/images/layouts/custom-navbar/logo.svg"
        alt="Flamelean's Logo"
        width="150"
        height="34"
      />
    </div>
    <div class="container d-flex flex-column align-items-center text-center py-5">
      <div class="col-12 col-xl-10">
        <progress-bar class="mb-4" width="w-75"/>
      </div>
      <h1 class="text-white mb-4">
        <span class="fw-bold">OH NO!</span> YOU JUST MISSED<br/>
        HUGE OPPORTUNITY
      </h1>
      <div class="text-white fs-5 fw-bold">
        But We Are Still Here To OFFER YOU ONE MORE AMAZING DISCOUNT...
      </div>
    </div>
  </section>
</template>

<script>
import ProgressBar from "@/components/ProgressBar.vue";

export default {
  name: "HeroSection",
  components: {ProgressBar}
}
</script>

<style scoped>

</style>
