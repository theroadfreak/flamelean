<template>
  <section>
    <title-text :title="title"
                :text="text"
    />
    <offer-section :bg-color="true"/>
  </section>
</template>

<script>
import TitleText from "@/components/footer-pages/TitleText";
import OfferSection from "@/components/index/OfferSection";
export default {
  name: "LabelSection",
  components: {OfferSection, TitleText},
  data() {
    return{
      title: 'FlameLean Label',
      text: 'Discover the FlameLean label which shows you one of the world\'s first, natural solutions to fix a newly discovered, scientifically proven cause of your belly fat and slow metabolism, low inner body temperature. Each ingredient found on the FlameLean label is clinically proven to support healthy weight loss levels. As always, I advise you to show a bottle of this to your doctor before you take it, just to be safe.',
    }
  }
}
</script>

<style scoped>

</style>
