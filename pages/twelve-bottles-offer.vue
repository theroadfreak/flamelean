<template>
  <main>
    <hero-section/>
    <title-subtitle-text class="py-5"
                         :title="wayToRegainControl.title"
                         :subtitle="wayToRegainControl.subtitle"
                         :text="wayToRegainControl.text"
    />
    <title-subtitle-text class="pb-5"
      :title="guaranteeLongLastingResults.title"
      subtitle=""
      :text="guaranteeLongLastingResults.text"
    />
    <special-offer-intro/>
    <product-offer-section :card="card" />
    <features-section/>
    <what-you-need-to-do-section yes="https://flamelean.pay.clickbank.net/?cbitems=12bottlesflameleanupsell&cbur=a" no="https://flamelean.pay.clickbank.net/?cbitems=12bottlesflameleanupsell&cbur=d"/>
  </main>
</template>

<script>
import HeroSection from "@/components/twelve-bottles-offer/HeroSection";
import TitleSubtitleText from "@/components/TitleSubtitleText";
import SpecialOfferIntro from "@/components/twelve-bottles-offer/SpecialOfferIntro";
import ProductOfferSection from "@/components/ProductOfferSection";
import FeaturesSection from "@/components/FeaturesSection";
import WhatYouNeedToDoSection from "@/components/twelve-bottles-offer/WhatYouNeedToDoSection";

export default {
  name: "twelve-bottles-offer",
  layout: 'no-navbar',
  components: {
    WhatYouNeedToDoSection,
    FeaturesSection, ProductOfferSection, SpecialOfferIntro, TitleSubtitleText, HeroSection},
  data() {
    return {
      title: '12 Bottles Offer | Flamelean',
      wayToRegainControl: {
        title: `Keep Reading: #1 Way To Regain Control Of
      Your Blood Sugar & Burn The Most Fat`,
        subtitle: `Don’t exit out of this page or hit the back button as it may cause
      errors to your order`,
        text: `Hey, Jessica here, and I’m so proud of you!<br class="d-none d-lg-flex"/>
      Once you start using FlameLean, there isn’t a single part of your life that won’t get better.<br
      class="d-none d-lg-flex"/>
      As your body begins to start normalising your blood sugar levels and help you feeling fuller for longer…<br
      class="d-none d-lg-flex"/>
      You’ll have a newfound confidence and feel like you’ve finally pressed your life’s “play” button.<br
      class="d-none d-lg-flex"/>
      Best of all, you’ll no longer feel insecure about what to wear, as you notice your body looking better than it
      ever<br class="d-none d-lg-flex"/>
      has before.<br/>
      Your friends and family will notice you’re not as tired anymore. Instead, you’ll been transforming into a livelier
      and<br class="d-none d-lg-flex"/>
      happier person that everyone wants to be around.<br class="d-none d-lg-flex"/>
      But before you start your transformation, I have something so important to share with you…`
      },
      guaranteeLongLastingResults: {
        title: `Unusual Way You Can Guarantee
Long-Lasting Results With FlameLean`,
        subtitle: '',
        text: `For the absolute best experience…<br class="d-none d-lg-flex"/>
It’s important to use FlameLean consistently because its effects compound over time.<br class="d-none d-lg-flex"/>
The more you take the faster you’ll normalise blood sugar levels…<br class="d-none d-lg-flex"/>
The better your body will be at using food for energy instead of storing it away as stubborn fast…<br class="d-none d-lg-flex"/>
And most importantly, the happier YOU will be!<br class="d-none d-lg-flex"/>
The problem though is that most of our customers tend to order FlameLean in bulk.<br class="d-none d-lg-flex"/>
Which means…`
      },
      card: {
        quantity: 12,
        price: 399,
        img: 'twelve-bottles-offer/flamelean-product.png',
        alt: 'Twelve bottles of Flamelean',
        perDay: 1.09,
        savings: 309,
      }
    }
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "og:title",
          property: "og:title",
          content: this.title,
        },
      ],
    };
  },
}
</script>

<style scoped>

</style>
