<template>
  <section
    class="container pb-5 d-flex flex-column align-items-center text-center text-black"
  >
    <h5 class="fw-bold mb-4">
      Like Billionaire Kim Kardashian… The Biggest Suspect To Be On It Right
      Now…
    </h5>
    <div class="col-12 col-lg-9 col-xxl-7 mb-5">
      <div class="ratio ratio-3x2">
        <img
          src="../../assets/images/tsl/the-biggest-suspect-section/kim-kardashian-transformation.png"
          class="object-fit-contain"
          alt="Kim Kardashian's transformation"
        />
      </div>
    </div>
    <title-subtitle-text class="mb-4" :text="text" />
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";

export default {
  name: "TheBiggestSuspectSection",
  components: { TitleSubtitleText },
  data() {
    return {
      text: `<span class="fw-bold">The thing is, this medication isn’t for the faint-hearted.<br class="d-none d-md-flex" />
It has to be injected once weekly in either the thigh, stomach, or upper arm.<br class="d-none d-md-flex" />
I should know.
Because as soon as my doctor told me about the medication…<br />
I practically begged him for a prescription.</span>`,
    };
  },
};
</script>

<style scoped></style>
