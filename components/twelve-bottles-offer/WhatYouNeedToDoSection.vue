<template>
  <section>
    <title-subtitle-text class="py-5"
                         :title="title"
                         :text="text"
    />
    <div class="container d-flex flex-column align-items-center text-center pb-5">
      <div class="col-11 col-sm-10 col-lg-7 col-xl-6 mb-4">
        <button
          class="w-100 btn btn-primary text-white py-3 rounded rounded-3 d-flex align-items-center justify-content-center text-center">
            <span class="fw-bold">
              <img src="../../assets/images/shopping-cart-icon.svg"
                   width="30"
                   height="26"
                   alt="Shopping Cart icon"
                   class="me-2"
              />
              YES, UPGRADE MY ORDER!</span>
        </button>
      </div>
      <div class="col-11 col-sm-9 col-lg-6 col-xl-5 text-primary">
        No, thanks, Jessica! I don’t want to get continued benefits from
        FlameLean to balance my blood sugar or lose any more weight.
      </div>
    </div>
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/twelve-bottles-offer/TitleSubtitleText";

export default {
  name: "WhatYouNeedToDoSection",
  components: {TitleSubtitleText},
  data() {
    return {
      title: `Here’s What You Need To Do Now`,
      text: `If you’d like to upgrade your order and get 12 bottles at a massive discount of $399 then simply<br class="d-none d-lg-flex" />
click the “Yes, Upgrade My Order” button below.<br class="d-none d-lg-flex" />
If you choose not to upgrade, that’s fine.<br class="d-none d-lg-flex" />
Just keep in mind that you will NOT be able to upgrade at this price for 12 bottles after you leave this page.<br class="d-none d-lg-flex" />
Remember, when you upgrade your entire order will be backed by our 180 days 100% money-back guarantee.<br class="d-none d-lg-flex" />
If you don’t experience the incredible results, simply return the bottles and we’ll give you a full refund.<br class="d-none d-lg-flex" />
So you see, you’ve got nothing to lose by upgrading your order.<br class="d-none d-lg-flex" />
Simply click the “Yes, Upgrade My Order” button below.`
    }
  }
}
</script>

<style scoped>

</style>
