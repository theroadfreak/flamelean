<template>
  <section class="bg-primary">
    <div class="py-5">
      <title-subtitle-text class="mb-5" title="Until I found the ONE thing that switches “on” your
fat burning hormone and effortlessly regulates
your blood sugar levels." :text="texts[0]" text-color="text-white"/>
      <title-subtitle-text title="Here’s Where Things Started To Go Terribly Wrong…"
                           :text="texts[1]" text-color="text-white"/>
    </div>
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";

export default {
  name: "ThingThatSwitchesOnFatBurningSection",
  components: {TitleSubtitleText},
  data() {
    return {
      texts: [
        `Even if you’ve struggled to lose weight your whole life…<br class="d-none d-lg-flex" />
Even if you’ve always planned your life around keeping your blood sugar levels in check…<br class="d-none d-lg-flex" />
And even if you’re 25, 45, or 65.<br class="d-none d-lg-flex" />
This natural miracle can help you turn your life around for the better.<br class="d-none d-lg-flex" />
But before I discovered it for myself…<br class="d-none d-lg-flex" />
I didn't think I’d ever control my blood sugar or lose weight with ease.<br class="d-none d-lg-flex" />
I was feeling so powerless.<br class="d-none d-lg-flex" />
So when I found out about this “holy grail” diabetes medication that celebrities were hoarding for themselves…<br class="d-none d-lg-flex" />
I was all on board.`,
        `My doctor didn’t hand over the prescription so readily.<br class="d-none d-lg-flex" />
Why?<br class="d-none d-lg-flex" />
Well, it turns out, some people shouldn’t take the medication at all.<br class="d-none d-lg-flex" />
Regardless of whether you have diabetes or not.<br class="d-none d-lg-flex" />
That’s because it comes with a boxed warning…<br class="d-none d-lg-flex" />
Which, I didn’t know at the time, but it’s the strongest safety-related warning required by the FDA.`
      ]
    }
  }
}
</script>

<style scoped>

</style>
