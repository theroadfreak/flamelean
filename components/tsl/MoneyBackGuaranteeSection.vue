<template>
  <section class="container d-flex flex-column align-items-center text-secondary text-center py-5">
    <h2 class="fw-bold mb-5 text-black">
      Your Investment Today Comes With The 180-Day<br class="d-none d-lg-flex"/>
      Money-Back Guarantee
    </h2>
    <title-subtitle-text class="mb-5" :text="texts[0]" text-color="text-black"/>
    <h2 class="text-center fw-bold mb-5 text-black">That’s Right, If You Don’t Think Your New Life Is…</h2>
    <flamelean-impact-features class="mb-4" title-color="text-black" :list="features"/>
    <title-subtitle-text :text="texts[1]" text-color="text-black"/>
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";
import FlameleanImpactFeatures from "@/components/FlameleanImpactFeatures";
export default {
  name: "MoneyBackGuaranteeSection",
  components: {FlameleanImpactFeatures, TitleSubtitleText},
  data() {
    return {
      texts: [
        `We get it, you’ve been stung before.<br class="d-none d-lg-flex"/>
There are so many supplements out there promising to get your blood sugar under control and help you drop a dress size.<br class="d-none d-lg-flex"/>
But the thing is, those supplements never switched on your fat-burning GLP-1 hormone.<br class="d-none d-lg-flex"/>
They didn’t make you full for much longer, suppress your cravings, or make you store fat and sugar in your body in the most optimal way.<br class="d-none d-lg-flex"/>
That’s why we aren’t just going to help you incinerate fat and optimize your blood sugar levels effortlessly.<br class="d-none d-lg-flex"/>
We’re going to guarantee it or your money back!`,
        `Then simply email us and we will give you 100% of your money back.<br class="d-none d-lg-flex"/>
No questions asked.<br class="d-none d-lg-flex"/>
And you have an entire 180 days to do this.<br class="d-none d-lg-flex"/>
Don’t sweat it, just send back the bottles and you don’t owe us a thing.<br class="d-none d-lg-flex"/>
That’s our pinky promise.<br class="d-none d-lg-flex"/>
Because honestly, we know you’re gonna love how you feel.<br class="d-none d-lg-flex"/>
Just like thousands of women before you.`
      ],
      features: [
        'Stress-free now your blood glucose levels are stable and rarely spike or crash',
        'A breeze now your body is able to use insulin more effectively, naturally',
        'Joyful because you’re no longer fighting a losing battle against carb and sugar cravings',
        'Energetic now the herbal blend is giving you a natural boost',
        'Super easy to lose weight because you’re fuller for longer and actually enjoy being active',
        'Empowering every time you’re told: “wow, you’ve lost so much weight - you look great!”',
        'The best it’s ever been now you’re finally in control of your blood sugar and weight…',
      ]
    }
  }
}
</script>

<style scoped>

</style>
