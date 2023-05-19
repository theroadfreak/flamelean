<template>
  <section class="bg-primary">
    <div class="py-5 text-white">
      <div v-for="effect in sideEffects" class="d-flex gap-3 justify-content-center mb-4">
        <div class="col-12 col-md-5">
          <div class="d-flex gap-1">
            <img
              v-if="effect.img !== null"
              :src="require('../../assets/images/tsl/medication-consequences-section/'+effect.img)"
              :alt="effect.img"
              width="45"
              height="45"
            >
            <h2 v-html="effect.title"></h2>
          </div>
          <ul>
            <li v-for="risk in effect.risks" v-html="risk"></li>
          </ul>
        </div>
        <img
          :src="require('../../assets/images/tsl/medication-consequences-section/'+effect.sideimage)"
          :alt="effect.sideimage"
          class="col-12 col-md-3"
        >

      </div>
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
      sideEffects: [
        {
          title: `The Medication Made Me Feel So Bad, I Couldn’t Raise My
Head To Vomit Into The Toilet Bowl!`,
          img: "pill.png",
          sideimage: "apcinja.png",
          risks: [
            'I was conflicted on what to do.',
            'I didn’t want to stop taking the drugs.',
            'Because it’s true what they say…',
            'I was losing weight easier than I’d ever done before.',
            'I was feelling fuller for longer.',
            'And I was able to keep my blood sugar levels stable without stressing like I did before.',
            'But there was no way I could stomach taking the medication anymore - literally.',
            'That’s when I went searching for a more natural alternative. I figured that…',
            'If I could find out WHY the medication worked so well at sabilizing my blood glucose levels…',
            'And helping me feel fuller for longer…',
            'Then maybe I could find a natural alternative that worked just as well - if not better!',
            'I became a little obsessed.',
            'I read through long reddit conversations about the medication…',
            'I researched scientific journals and studies that explained WHY it was so effective.',
          ],
        },
      ],
    }
  }
}
</script>

<style scoped>

</style>
