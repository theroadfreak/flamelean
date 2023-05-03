<template>
  <section class="text-center">
    <title-subtitle-text class="pt-5"
                         :title="title[0]"
    />
    <the-xed-list :list="commonSideEffects"/>
    <a href="https://www.singlecare.com/blog/ozempic-alternatives/" target="_blank" class="text-center text-4D4D4D text-decoration-none font-size-12px">
      https://www.singlecare.com/blog/ozempic-alternatives/
    </a>
    <title-subtitle-text class="pt-5"
                         :title="title[1]"
    />
    <the-xed-list :list="risks" class="mb-3"/>
    <title-subtitle-text class="pb-5"
                         :text="text"
                         text-color="text-black"
    />
  </section>
</template>

<script>
import TitleSubtitleText from "~/components/TitleSubtitleText";
import TheXedList from "@/components/tsl/CommonSideEffects/TheXedList";
export default {
  name: "CommonSideEffectsSection",
  components: {TheXedList, TitleSubtitleText},
  data() {
    return {
      title: [
        `My Doctor Made Me Aware Of The<br class="d-none d-sm-flex" />
Common Side Effects, Like:`,
        `And Then The More Serious Risks, Like:`,
      ],
      commonSideEffects: [
        'Nausea...',
        'Stomach Pain...',
        'Vomiting...',
        'And stomach pain...'
      ],
      risks: [
        'Kidney problems...',
        'Pancreatitis...',
        'Gallstones...',
        'Or severe allergic reactions'
      ],
      text: `But all I could think about were the ads I was seeing everywhere…<br class="d-none d-lg-flex" />
Promising to lose on average up to 12 pounds.<br class="d-none d-lg-flex" />
So, I decided to take my chances and went ahead with the prescription.<br class="d-none d-lg-flex" />
And girl, that was the wrong move!<br class="d-none d-lg-flex" />
Because during those 5 weeks of injecting myself with the medication…<br class="d-none d-lg-flex" />
I couldn’t move from the bathroom floor!<br class="d-none d-lg-flex" />
I was vomiting so much I didn’t even have the energy to get up.<br class="d-none d-lg-flex" />
Yep - I was basically lying in my own puke.<br class="d-none d-lg-flex" />
Gross, I know.`,
    }
  }
}
</script>

<style scoped>

</style>
