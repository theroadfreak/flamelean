<template>
  <section class="bg-primary">
  <div class="container">
    <div class="py-5">
      <div class="d-flex justify-content-center">
        <div class="col-12 col-md-7">
            <h2 class="text-white fw-bold mb-3">Until I found the ONE thing that switches “on” your
              fat burning hormone and effortlessly regulates
              your blood sugar levels.</h2>
          <ul class="text-white">
            <li v-for="item in texts" v-html="item"></li>
          </ul>
        </div>
      </div>
    </div>
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
        'Even if you’ve struggled to lose weight your whole life…',
        'Even if you’ve always planned your life around keeping your blood sugar levels in check…<br class="d-none d-lg-flex" And even if you’re 25, 45, or 65.',
        '<span class="fw-bold">This natural miracle can help you turn your life around for the better. But before I discovered it for myself… </span>',
        'I didn’t think I’d ever control my blood sugar or lose weight with ease. I was feeling so powerless.',
        'So when I found out about this “holy grail” diabetes medication that celebrities were hoarding for themselves… I was all on board.',
      ],

    }
  }
}
</script>

<style scoped>

</style>
