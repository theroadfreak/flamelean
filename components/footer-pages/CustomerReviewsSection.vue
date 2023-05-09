<template>
<title-text :title="title"
            :text="text"
/>
</template>

<script>
import TitleText from "@/components/footer-pages/TitleText";
export default {
  name: "CustomerReviewsSection",
  components: {TitleText},
  data() {
    return{
      title: 'FlameLean Customer Reviews',
      text: 'We have already received over 215,000 FlameLean customer reviews from men and women around the world who have had life-changing results. Our target is to make that a million and we want you to be our next success story. Remember our FlameLean customer reviews recommend you take FlameLean for at least 3 to 6 months, so it has enough time to work throughout your entire body to target your inner body temperature, reach your desired weight, and lock it in for years into the future.\n'
    }
  }
}
</script>

<style scoped>

</style>
