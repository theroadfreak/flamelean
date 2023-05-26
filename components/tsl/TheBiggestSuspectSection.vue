<template>
  <section
    class="container pb-5 d-flex flex-column align-items-center text-center text-black"
  >
    <h5 class="fw-bold mb-4">
      Like Billionaire Kim Kardashian… The Biggest Suspect To Be On It Right
      Now…
    </h5>
    <div class="col-12 col-md-6 mb-5">
      Celebrities are now getting these diabetes medications easily prescribed
      to them…<br class="d-none d-lg-flex" />
      <p class="mb-0">
        <span class="fw-bold text-danger text-decoration-underline"
          >Paying a hefty $1,300 fee every single month.</span
        ><br class="d-none d-md-flex" />
      </p>

      <p class="mb-0">
        <span class="fst-italic"> It costs as much as many mortgages!</span>
        Because of that, most insurance companies won’t cover it for regular
        folk like you and me. And while the price might be eye watering to us.
        It’s a drop in the ocean for the rich and famous. Meaning they can
        easily achieve rapid weight loss and keep it off. So long as they
        continue injecting themselves with the medication. <br />
        Celebrities are now getting these diabetes medications easily prescribed
        to them…<br class="d-none d-lg-flex" />
      </p>

      <p>
        <span class="fw-bold"
          >After she mysteriously lost 16 pounds in just 3 weeks to fit into
          Marilyn Monroe’s dress.</span
        >
      </p>
    </div>
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
