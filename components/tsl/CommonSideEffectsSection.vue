<template>
  <section class="my-4 px-3 px-md-4">
    <div class="d-flex justify-content-center mb-4">
      <div class="col-12 col-md-6">
        <h2 class="fw-bold mb-3">❌ Here’s Where Things Started To Go Terribly Wrong…</h2>
        <ul>
          <li v-for="item in texts" v-html="item"></li>
        </ul>
      </div>
    </div>
    <div class="d-flex flex-column align-items-center">
      <div v-for="effect in sideEffects" class="col-12 col-md-6 mb-4">
        <div class="d-flex gap-1">
          <img
            v-if="effect.img !== null"
            :src="require('../../assets/images/tsl/common-side-effects-section/'+effect.img)"
            :alt="effect.img"
            width="45"
            height="45"
          >
          <h2 class="fw-bold mb-3" v-html="effect.title"></h2>
        </div>
        <ul>
          <li v-for="risk in effect.risks" v-html="risk"></li>
        </ul>
      </div>
    </div>

  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";

export default {
  name: "CommonSideEffectsSection",
  components: {TitleSubtitleText},
  data() {
    return {
      texts: [
        'My doctor didn’t hand over the prescription so readily. <span class="fw-bold">WHY?</span>',
        'Well, it turns out, some people shouldn’t take the medication at all.',
        'Regardless of whether you have diabetes or not.',
        'That’s because it comes with a boxed warning…',
        'Which, I didn’t know at the time, but it’s the strongest safety-related warning required by the FDA.',
      ],
      sideEffects: [
        {
          title: `My Doctor Made Me Aware Of The
                    Common Side Effects, Like:`,
          img: "doctor.png",
          risks: [
            'Nausea...',
            'Stomach Pain...',
            'Vomiting...',
            'And stomach pain...'
          ],
        },
        {
          title: `And Then The More Serious Risks, Like:`,
          img: null,
          risks: [
            '<span class="fw-bold">Kidney problems...</span>',
            '<span class="fw-bold">Pancreatitis...</span>',
            '<span class="fw-bold">Gallstones...</span>',
            '<span class="fw-bold">Or severe allergic reactions</span>'
          ],
        }
      ],
    }
  }
}
</script>

<style scoped>

</style>
