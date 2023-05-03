<template>
  <section class="bg-primary">
    <div class="container py-5 text-center d-flex flex-column align-items-center text-white">
      <h2 class="fw-bold mb-5">
        No Other Natural Solution Has Come Close<br class="d-none d-lg-flex"/>
        To Producing This Level Of Weight Loss And<br class="d-none d-lg-flex"/>
        Blood Glucose Support…
      </h2>
      <h2 class="fw-bold mb-5">
        This Really Is A Game-Changer!
      </h2>
      <div class="mb-4">Consider this...</div>
      <title-subtitle-text :text="text" text-color="text-white"/>
    </div>
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";

export default {
  name: "NaturalSolutionSection",
  components: {TitleSubtitleText},
  data() {
    return {
      text: `
Just ONE of those 4 ingredients would support healthy blood glucose levels<br class="d-none d-lg-flex" />
 and trigger long-lasting weight loss.<br class="d-none d-lg-flex" />
Now picture uniting all of them in the scientifically-proven amounts…<br class="d-none d-lg-flex" />
And adding 15 other well-researched botanicals, nutrients, and minerals to<br class="d-none d-lg-flex" />
 boost and accelerate your transformation even more.<br class="d-none d-lg-flex" />
That's precisely what we've created – and it's the reason our customers are<br class="d-none d-lg-flex" />
 looking and feeling incredible!`
    }
  }
}
</script>

<style scoped>

</style>
