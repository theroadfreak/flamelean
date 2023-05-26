<template>
  <main>
    <div class="bg-primary">
      <div class="container py-5">
        <h1 class="text-white text-center">Thank You for your order!</h1>
        <h3 class="text-white text-center">
          Your credit card statement will show a charge from CLKBANK!
        </h3>
      </div>
    </div>

    <div
      class="container d-flex flex-column flex-wrap align-content-center justify-content-center"
    >
      <h4 class="py-5 col-12 col-md-6">
        Your package will be shipped in next 3-5 business days. if you have any
        questions you can contact us on
        <a href="mailto:support@flamelean.com">support@flamelean.com</a>
      </h4>
      <div class="mx-auto mb-5">
        <nuxt-link
          to="/"
          class="btn btn-primary px-3 fs-4 rounded rounded-3 shadow-lg"
        >
          <p class="text-white mb-0">Back to home</p>
        </nuxt-link>
      </div>
    </div>
    <div
      class="container d-flex flex-column flex-wrap align-content-center justify-content-center"
    >
      <h4 class="py-5">
        Testimonials, case studies, and examples found on this page are results
        that have been forwarded to us by users of FLAMELEAN products and
        related products are not intended to represent or guarantee that anyone
        will achieve the same or similar results.
      </h4>
    </div>
    <div class="my-5 py-5"></div>
  </main>
</template>

<script>
export default {
  name: "thank-you",
  layout: "no-navbar",
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "og:title",
          property: "og:title",
          content: this.title,
        },
      ],
    };
  },
};
</script>

<style scoped></style>
