<template>
  <section>
    <title-subtitle-text class="py-5" :title="title" :text="text" />
  </section>
</template>

<script>
import TitleSubtitleText from "@/components/TitleSubtitleText";

export default {
  name: "WhatYouNeedToDoSection",
  components: { TitleSubtitleText },
  props: {
    yes: {
      type: String,
      required: true,
    },
    no: {
      type: String,
      required: true,
    },
  },
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
Simply click the “Yes, Upgrade My Order” button below.`,
    };
  },
};
</script>

<style scoped></style>
