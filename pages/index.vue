<template>
  <main>
    <hero-section/>
    <stanford-scientists-article-section/>
    <flamelean-carnitine-substance-section/>
  </main>
</template>

<script>
import HeroSection from "@/components/index/HeroSection.vue";
import StanfordScientistsArticleSection from "@/components/index/StanfordScientistsArticleSection.vue";
import FlameleanCarnitineSubstanceSection from "@/components/index/FlameleanCarnitineSubstanceSection.vue";

export default {
  name: 'IndexPage',
  components: {FlameleanCarnitineSubstanceSection, StanfordScientistsArticleSection, HeroSection}
}
</script>
