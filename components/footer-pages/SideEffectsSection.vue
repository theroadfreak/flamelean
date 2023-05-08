<template>
  <section>
    <title-text :title="title"
                :text="text"
    />
    <frequently-asked-questions-section/>
  </section>
</template>

<script>
import TitleText from "@/components/footer-pages/TitleText";
import FrequentlyAskedQuestionsSection from "@/components/index/FrequentlyAskedQuestionsSection";
export default {
  name: "SideEffectsSection",
  components: {FrequentlyAskedQuestionsSection, TitleText},
  data() {
    return{
      title: 'FlameLean Side Effects',
      text: 'FlameLean is a proprietary natural formula manufactured in the USA at our FDA registered and GMP certified facility using state of the art, precision engineered machinery and under the strictest and most sterile standards.\n' +
        'Each ingredient is 100% plant-based, soy-free, dairy-free, non-GMO, and put through additional third-party inspections and quality control to ensure high purity and potency.\n' +
        'A common side effect from FlameLean is having to toss your baggy clothes in the trash and spend hours in the dressing room trying on new sexy tight-fitting clothes. As always, I advise you to show a bottle of this to your doctor before you take it, just to be safe.\n'
    }
  }
}
</script>

<style scoped>

</style>
