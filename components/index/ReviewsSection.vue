<template>
  <section class="container d-flex flex-column align-items-center pt-5">
    <h2 class="text-center text-secondary fw-bold mb-5">
      Real Flamelean Users.<br />
      Real Life-Changing Results.
    </h2>
    <div class="row d-flex justify-content-center mt-md-4">
      <div
        v-for="(review, i) in reviews"
        :key="i"
        class="col-11 col-sm-8 col-md-5 col-xl-4 mb-5"
        :class="{ 'offset-md-1': i % 2 !== 0 }"
      >
        <review :review="review" />
      </div>
    </div>
  </section>
</template>

<script>
import Review from "@/components/index/ReviewsSection/Review";

export default {
  name: "ReviewsSection",
  components: { Review },
  data() {
    return {
      reviews: [
        {
          title: "Deborah is 34 lbs lighter so far...",
          paragraph: `I started using this -- two tablespoons in the morning and two in mid-afternoon. I have lost 40
            lbs in just a few months and plan to lose another 15 to get to my ideal body weight of around 210. I am 6'2"
            tall, age 58. I workout regularly 1 hour of cardio 5 x a week and 30 minutes of weights 3 days per week.
            This is an amazing supplement.`,
        },
        {
          title: "Deborah is 34 lbs lighter so far...",
          paragraph: `I started using this -- two tablespoons in the morning and two in mid-afternoon. I have lost 40
            lbs in just a few months and plan to lose another 15 to get to my ideal body weight of around 210. I am 6'2"
            tall, age 58. I workout regularly 1 hour of cardio 5 x a week and 30 minutes of weights 3 days per week.
            This is an amazing supplement.`,
        },
        {
          title: "Deborah is 34 lbs lighter so far...",
          paragraph: `I started using this -- two tablespoons in the morning and two in mid-afternoon. I have lost 40
            lbs in just a few months and plan to lose another 15 to get to my ideal body weight of around 210. I am 6'2"
            tall, age 58. I workout regularly 1 hour of cardio 5 x a week and 30 minutes of weights 3 days per week.
            This is an amazing supplement.`,
        },
        {
          title: "Deborah is 34 lbs lighter so far...",
          paragraph: `I started using this -- two tablespoons in the morning and two in mid-afternoon. I have lost 40
            lbs in just a few months and plan to lose another 15 to get to my ideal body weight of around 210. I am 6'2"
            tall, age 58. I workout regularly 1 hour of cardio 5 x a week and 30 minutes of weights 3 days per week.
            This is an amazing supplement.`,
        },
      ],
    };
  },
};
</script>

<style scoped></style>
