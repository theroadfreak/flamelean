<template>
  <section class="bg-primary">
    <div class="pb-5">
      <title-subtitle-text class="pt-5"
                           :title="medicationEffects.title"
                           :text="medicationEffects.text"
                           text-color="text-white"

      />
      <title-subtitle-text class="pt-5"
                           :title="theTruth.title"
                           :text="theTruth.text"
                           text-color="text-white"
      />
    </div>
  </section>
</template>

<script>
import TitleSubtitleText from "~/components/TitleSubtitleText";

export default {
  name: "MedicationConsequencesSection",
  components: {TitleSubtitleText},
  data() {
    return {
      medicationEffects: {
        title: `The Medication Made Me Feel So Bad, I Couldn’t Raise My
Head To Vomit Into The Toilet Bowl!`,
        text: `I was conflicted on what to do.<br class="d-none d-lg-flex" />
I didn’t want to stop taking the drugs.<br class="d-none d-lg-flex" />
Because it’s true what they say…<br class="d-none d-lg-flex" />
I was losing weight easier than I’d ever done before.<br class="d-none d-lg-flex" />
I was feelling fuller for longer.<br class="d-none d-lg-flex" />
And I was able to keep my blood sugar levels stable without stressing like I did before.<br class="d-none d-lg-flex" />
But there was no way I could stomach taking the medication anymore - literally.<br class="d-none d-lg-flex" />
That’s when I went searching for a more natural alternative.<br class="d-none d-lg-flex" />
I figured that…<br class="d-none d-lg-flex" />
If I could find out WHY the medication worked so well at sabilizing my blood glucose levels…<br class="d-none d-lg-flex" />
And helping me feel fuller for longer…<br class="d-none d-lg-flex" />
Then maybe I could find a natural alternative that worked just as well - if not better!<br class="d-none d-lg-flex" />
I became a little obsessed.<br class="d-none d-lg-flex" />
I read through long reddit conversations about the medication…<br class="d-none d-lg-flex" />
I researched scientific journals and studies that explained WHY it was so effective.`
      },
      theTruth: {
        title: `Here’s The TRUTH I Discovered That Helped Me
Lose 40 Pounds In Less Than 2 Months…`,
        text: `The diabetes medication the rich and famous are hoarding right now…<br class="d-none d-lg-flex" />
Releases a chemical in your body that mimics a hormone.<br class="d-none d-lg-flex" />
This hormone is called GLP-1…<br class="d-none d-lg-flex" />
Which stands for glucagon-like peptide-1.<br class="d-none d-lg-flex" />
I won’t bore you with the complicated scientific details, but…`
      }
    }
  }
}
</script>

<style scoped>

</style>
