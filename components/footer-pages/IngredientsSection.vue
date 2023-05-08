<template>
<section>
  <title-text :title="title"
              :text="text"
  />
  <flamelean-ingredients-section/>
</section>
</template>

<script>
import TitleText from "@/components/footer-pages/TitleText";
import FlameleanIngredientsSection from "@/components/FlameleanIngredientsSection";
export default {
  name: "IngredientsSection",
  components: {FlameleanIngredientsSection, TitleText},
  data(){
    return{
      title: 'FlameLean Ingredients',
      text: 'Inside every capsule is FlameLean ingredients of a bespoke proprietary formula of 6 high-quality alpine nutrients and plants, in the exact clinically proven quantities, that work on a biological level to target inner body temperature. By targeting your inner body temperature you are effortlessly waking up and electrifying your metabolism, your calories burning engine! So even when sleeping or lying on the couch, the special FlameLean ingredients means you\'re dissolving the deepest most stubborn fat from every nook and cranny of your entire body into pure, natural all-day energy. As always, I advise you to show a bottle of this to your doctor before you take it, just to be safe.\n'
    }
  }
}
</script>

<style scoped>

</style>
