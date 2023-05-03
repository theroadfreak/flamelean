<template>
  <section class="container d-flex flex-column align-content-center">
    <h2 class="text-secondary text-center fw-bold py-4">The Most Important Thing You Need To Know Is…</h2>
    <flamelean-impact-features :list="mostImportantThings" title-color="text-secondary" class="mb-5"/>
    <h4 class="text-black text-center fw-bold mb-4">That’s because GLP-1 works in 3 ways:</h4>
    <div class="text-center mb-3 text-black">
      <ul v-for="(way, i) in ways" :key="i" class="list-unstyled">
        <li>{{ way }}</li>
      </ul>
    </div>
    <title-subtitle-text :text="text"
                         class="pb-5"
                         text-color="text-black"
    />
  </section>
</template>

<script>
import FlameleanImpactFeatures from "~/components/FlameleanImpactFeatures";
import TitleSubtitleText from "~/components/TitleSubtitleText";

export default {
  name: "TheMostImportantThingSection",
  components: {TitleSubtitleText, FlameleanImpactFeatures},
  data() {
    return {
      mostImportantThings: [
        'GLP-1 is responsible for making you feel fuller for much longer…',
        'Have zero cravings for sweet and salty foods…',
        'And store fat and sugar in your body in a more flattering way'
      ],
      ways: [
        '1. By helping your pancreas release insulin when blood sugar levels are high…',
        '2. Helping move sugar out of your blood and into other body tissues to be used for energy instead of stored as fat…',
        '3. Slowing the movement of food through the stomach to decrease appetite and lose weight…'
      ],
      text: `The science proves it!<br class="d-none d-lg-flex"/>
A lead Doctor at one of London’s most prestigious health science centres, confirms that…<br class="d-none d-lg-flex"/>
When most people eat, their GLP-1 levels go up…<br class="d-none d-lg-flex"/>
Which helps them feel satisfied and use food as energy, instead of storing it as fat.<br class="d-none d-lg-flex"/>
But patients with Type 2 diabetes lack this.<br class="d-none d-lg-flex"/>
Their GLP-1 levels stay the same…<br class="d-none d-lg-flex"/>
Which means your food isn’t moving out of your blood into your body…<br class="d-none d-lg-flex"/>
But instead, staying inside your bloodstream…<br class="d-none d-lg-flex"/>
Causing your blood sugar levels to become imbalanced…<br class="d-none d-lg-flex"/>
Making you feel slow and sluggish, like you’re running on an empty tank!<br class="d-none d-lg-flex"/>
That’s why this 3-step function of the medication works so well for people with diabetes…<br class="d-none d-lg-flex"/>
Because it helps your pancreas release the right amount of insulin…<br class="d-none d-lg-flex"/>
Which, your body isn’t equipped to do optimally on its own.`,
    }
  }
}
</script>

<style scoped>

</style>
