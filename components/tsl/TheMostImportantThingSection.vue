<template>
  <section class="container d-flex flex-column align-content-center">
    <title-subtitle-text
      :title="theTruth.title"
      :text="theTruth.text"
      class="py-5"
      text-color="text-black"
    />
    <flamelean-impact-features
      :features="mostImportantThings"
      title-color="text-danger"
      title="The Most Important Thing You Need To Know Is…"
      class="my-5"
    />
    <div class="row">
      <div class="col-12 col-md-6">
        <h5 class="text-black text-center fw-bold mb-4">
          That’s because GLP-1 works in 3 ways:
        </h5>
        <div class="mb-3 text-black">
          <ul class="list-unstyled">
            <li v-for="(way, i) in ways" :key="i" class="mb-2">
              <div v-html="way"></div>
            </li>
          </ul>
        </div>
      </div>

      <div class="col-12 col-md-3 mx-auto mb-5">
        <div style="">
          <iframe
            src="https://player.vimeo.com/video/828611662?h=810b75824d&title=0&byline=0"
            style="
              position: absolute;
              top: 0;
              left: 0;
              width: 100%;
              height: 100%;
            "
            frameborder="0"
            allow="autoplay; fullscreen; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
        <!-- <script src="https://player.vimeo.com/api/player.js"></script> -->
      </div>
    </div>
  </section>
</template>

<script>
import FlameleanImpactFeatures from "~/components/FlameleanImpactFeatures";
import TitleSubtitleText from "~/components/TitleSubtitleText";

export default {
  name: "TheMostImportantThingSection",
  components: { TitleSubtitleText, FlameleanImpactFeatures },
  data() {
    return {
      theTruth: {
        title: `Here’s The TRUTH I Discovered That Helped Me
Lose 40 Pounds In Less Than 2 Months…`,
        text: `The diabetes medication the rich and famous are hoarding right now…<br class="d-none d-lg-flex" />
Releases a chemical in your body that mimics a hormone.<br class="d-none d-lg-flex" />
This hormone is called GLP-1…<br class="d-none d-lg-flex" />
Which stands for glucagon-like peptide-1.<br class="d-none d-lg-flex" />
I won’t bore you with the complicated scientific details, but…`,
      },
      mostImportantThings: [
        "GLP-1 is responsible for making you feel fuller for much longer…",
        "Have zero cravings for sweet and salty foods…",
        "And store fat and sugar in your body in a more flattering way",
      ],
      ways: [
        "Helping move sugar out of your blood and into other body tissues to be used for energy instead of stored as fat…",
        'Slowing the movement of food through the stomach to decrease appetite and lose weight… <br> <span class="fw-bold"> The science proves it! </span> A lead Doctor at one of London’s most prestigious health science centres, confirms that…<br> When most people eat, their <span class="fw-bold"> GLP-1 levels go up…</span> ',
        '<span class="fw-bold"> But patients with Type 2 diabetes lack this.</span> Their GLP-1 levels stay the same. Which means your food isn’t moving out of your blood into your body. But instead, staying inside your bloodstream. Causing your blood sugar levels to become imbalanced. <span class="fw-bold"> Making you feel slow and sluggish, like you’re running on an empty tank! </span>',
        '<span class="fw-bold">That’s why this 3-step function of the medication works so well for people with diabetes… Because it helps your pancreas release the right amount of insulin. Which, your body isn’t equipped to do optimally on its own. </span>',
      ],
    };
  },
  mounted() {
    const scriptEl = document.createElement("script");
    scriptEl.type = "text/javascript";
    scriptEl.src = "https://player.vimeo.com/api/player.js";
    document.body.appendChild(scriptEl);
    scriptEl.defer = true;
  },
};
</script>

<style scoped>
/*.responsive-iframe-container {*/
/*  position: relative;*/
/*  overflow: hidden;*/
/*  padding: 177.78%;*/
/*}*/

/*.responsive-iframe {*/
/*  position: absolute;*/
/*  top: 0;*/
/*  left: 0;*/
/*  width: 100%;*/
/*  height: 100%;*/
/*}*/
</style>
