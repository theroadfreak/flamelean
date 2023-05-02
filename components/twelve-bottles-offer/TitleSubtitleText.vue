<template>
  <section class="container d-flex flex-column align-items-center text-center">
    <h2 class="fw-bold col-12 col-lg-10 col-xl-8 line-height-normal mb-3" :class="textColor" v-html="title">
    </h2>
    <h5 class="text-danger col-11 col-lg-9 col-xl-7 mb-4">
      {{ subtitle }}
    </h5>
    <div :class="textColor" v-html="text"></div>
  </section>
</template>

<script>
export default {
  name: "TitleSubtitleText",
  props: {
    title: {
      type: String,
      default: '',
    },
    subtitle: {
      type: String,
      default: '',
    },
    text: {
      type: String,
      default: '',
    },
    textColor: {
      type: String,
      default: 'text-secondary',
    }
  }
}
</script>

<style scoped>

</style>
