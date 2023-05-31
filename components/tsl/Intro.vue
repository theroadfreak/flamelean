<template>
  <section
    class="container d-flex flex-column align-items-center text-center py-5"
  >
    <!-- <as-talked-about-in-section /> -->
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";
// import AsTalkedAboutInSection from "@/components/AsTalkedAboutInSection";

export default {
  name: "Intro",
  components: { /*AsTalkedAboutInSection,*/ TitleSubtitleText },
  data() {
    return {
      texts: [
        `Celebrities are now getting these medications for normal blood sugar level...
        <br class="d-none d-lg-flex" />
        <span class="fw-bold text-danger text-decoration-underline">
          Paying a hefty $1,300 fee every single month.
        </span>
        <br class="d-none d-md-flex" />
        <span class="fst-italic">
          It costs as much as many mortgages!
        </span>
        <br class="d-none d-md-flex" />
        Because of that, most insurance companies won’t cover it for regular folk like you and me.
        <br class="d-none d-md-flex" />
        And while the price might be eye watering to us…`,
        `It’s a drop in the ocean for the rich and famous.
        <br class="d-none d-md-flex" />
        Meaning they can easily achieve rapid weight loss and keep it off…
        <br class="d-none d-md-flex" />
        So long as they continue injecting themselves with the medication.`,
      ],
    };
  },
};
</script>

<style scoped></style>
