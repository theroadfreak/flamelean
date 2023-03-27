<template>
  <main>
    <hero-section/>
    <stanford-scientists-article-section/>
  </main>
</template>

<script>
import HeroSection from "@/components/index/HeroSection.vue";
import StanfordScientistsArticleSection from "@/components/index/StanfordScientistsArticleSection.vue";

export default {
  name: 'IndexPage',
  components: {StanfordScientistsArticleSection, HeroSection}
}
</script>
