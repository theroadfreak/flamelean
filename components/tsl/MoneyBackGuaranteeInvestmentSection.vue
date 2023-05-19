<template>
  <section class="container d-flex flex-column align-items-center text-secondary text-center py-5">
      <flamelean-impact-features class="mb-4"
                                 title-color="text-black"
                                 :features="features"
                                 title="That’s Right, If You Don’t Think Your New Life Is…"
      />
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";
import FlameleanImpactFeatures from "@/components/FlameleanImpactFeatures";

export default {
  name: "MoneyBackGuaranteeInvestmentSection",
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
