<template>
  <main>
    <title-text :title="title"
                :text="text"
    />
    <flamelean-features-section/>
  </main>
</template>

<script>
import TitleText from "@/components/footer-pages/TitleText";
import FlameleanFeaturesSection from "@/components/index/FlameleanFeaturesSection";
export default {
  name: "benefits",
  layout: 'footer-pages-layout',
  components: {FlameleanFeaturesSection, TitleText},
  data() {
    return{
      title:'FlameLean Benefits',
      text: 'FlameLean is the first product in the world clinically proven to rapidly target inner body temperature.Science has now proven that low inner body temperature is a real cause of your belly fat. By targeting inner body temperature you will wake up and electrify your sleeping metabolism, and set your calorie burning engine into overdrive! The incredible FlameLean benefits are too many to mention as you will have never experienced weight loss as effortlessly as with FlameLean. We know you will love the results that FlameLean has in store for you!'
    }
  }
}
</script>

<style scoped>

</style>
