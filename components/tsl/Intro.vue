<template>
  <section class="container d-flex flex-column align-items-center text-center py-5">
    <title-subtitle-text :text="texts[0]"/>
    <as-talked-about-in-section/>
    <title-subtitle-text class="mb-4" :text="texts[1]" text-color="text-black"/>
    <title-subtitle-text :text="texts[2]" text-color="text-black"/>
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";
import AsTalkedAboutInSection from "@/components/AsTalkedAboutInSection";

export default {
  name: "Intro",
  components: {AsTalkedAboutInSection, TitleSubtitleText},
  data() {
    return {
      texts: [
        `Because they’re deeply concerned - and you should be too.<br class="d-none d-md-flex" />
Celebrities like Elon Musk are abusing a prescription medication…<br class="d-none d-md-flex" />
Especially formulated for people with Type 2 diabetes like me (and maybe you).<br class="d-none d-md-flex" />
But these celebrities don’t have erratic blood sugar spikes…<br class="d-none d-md-flex" />
They’re not at risk of heart failure…<br class="d-none d-md-flex" />
Or having their leg amputated, like Type 2 diabetics.<br class="d-none d-md-flex" />
Instead, they’re stocking up on the severely limited drug…<br class="d-none d-md-flex" />
Just so they can lose weight.`,
        `Celebrities are now getting these diabetes medications easily prescribed to them…<br class="d-none d-lg-flex" />
Paying a hefty $1,300 fee every single month.<br class="d-none d-md-flex" />
It costs as much as many mortgages!<br class="d-none d-md-flex" />
Because of that, most insurance companies won’t cover it for regular folk like you and me.<br class="d-none d-md-flex" />
And while the price might be eye watering to us…`,
        `It’s a drop in the ocean for the rich and famous.<br class="d-none d-md-flex" />
Meaning they can easily achieve rapid weight loss and keep it off…<br class="d-none d-md-flex" />
So long as they continue injecting themselves with the medication.`
      ]
    }
  }
}
</script>

<style scoped>

</style>
