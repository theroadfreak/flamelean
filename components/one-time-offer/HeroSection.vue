<template>
  <section class="bg-primary">
    <div class="container d-flex flex-column align-items-center text-center py-5">
      <div class="col-12 col-xl-10">
        <progress-bar class="mb-4" width="w-50"/>
      </div>
      <h1 class="text-white mb-4">
        <span class="fw-bold">WAIT!</span> ONE TIME OFFER
      </h1>
      <div class="text-white fs-5 fw-bold">
        You Will Never See This Page Again!
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
