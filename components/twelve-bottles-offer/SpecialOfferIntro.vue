<template>
  <div class="bg-primary">
    <title-subtitle-text
      class="py-5"
      :title="outOfStock.title"
      :text="outOfStock.text"
      text-color="text-white"
    />
    <title-subtitle-text
      :title="specialOffer.title"
      :text="specialOffer.text"
      text-color="text-white"
    />
  </div>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";

export default {
  name: "SpecialOfferIntro",
  components: { TitleSubtitleText },
  data() {
    return {
      outOfStock: {
        title: `FlameLean Can Go<br class="d-none d-sm-flex" />
Out Of Stock For Months At A Time!`,
        text: `The last thing I want is for you to start experiencing a sense of confidence
         and control over your body…<br class="d-none d-lg-flex" />
Only to find out that we’re out of stock when you need more bottles!<br class="d-none d-lg-flex" />
That’s the bad news.`,
      },
      specialOffer: {
        title: `Here’s The Special Offer<br class="d-none d-sm-flex" />
I Have For You Today`,
        text: `<b>The regular price for a year supply of FlameLean is $468…</b><br class="d-none d-lg-flex" />
But since you’re a new customer, here’s what I’m offering you instead…`,
      },
    };
  },
};
</script>

<style scoped></style>
