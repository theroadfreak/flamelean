<template>
  <section class="container pb-5 d-flex flex-column align-items-center text-center text-black">
    <h2 class="fw-bold mb-4">Like Billionaire Kim Kardashian… The Biggest Suspect To<br class="d-none d-lg-flex"/>
      Be On It Right Now…</h2>
    <div class="mb-5">
      After she mysteriously lost 16 pounds in just 3 weeks to fit into Marilyn Monroe’s dress.
    </div>
    <div class="col-12 col-lg-9 col-xxl-7 mb-5">
      <div class="ratio ratio-3x2">
        <img src="../../assets/images/tsl/the-biggest-suspect-section/kim-kardashian-transformation.png"
             class="object-fit-contain"
             alt="Kim Kardashian's transformation"
        />
      </div>
    </div>
    <title-subtitle-text class="mb-4" :text="text"/>
    <a href="https://www.forbes.com/sites/ariannajohnson/2022/12/26/what-to-know-about-ozempic/?sh=24e00d9b5adb"
       class="text-4D4D4D text-decoration-none font-size-12px text-break"
    >
      https://www.forbes.com/sites/ariannajohnson/2022/12/26/what-to-know-about-ozempic/?sh=24e00d9b5adb
    </a>
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";

export default {
  name: "TheBiggestSuspectSection",
  components: {TitleSubtitleText},
  data() {
    return {
      text: `The thing is, this medication isn’t for the faint-hearted.<br class="d-none d-md-flex" />
It has to be injected once weekly in either the thigh, stomach, or upper arm.<br class="d-none d-md-flex" />
I should know.<br class="d-none d-md-flex" />
Because as soon as my doctor told me about the medication…<br class="d-none d-md-flex" />
I practically begged him for a prescription.`
    }
  }
}
</script>

<style scoped>

</style>
