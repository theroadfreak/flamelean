<template>
  <section class="container py-5">
    <div class="d-flex flex-column justify-content-center align-items-center text-center text-secondary mb-5">
      <h2 class="fw-bold mb-md-5">Inside Every Capsule Of FlameLean You’ll Also Find:</h2>
    </div>
    <div class="row d-flex justify-content-center justify-content-md-start">
      <div v-for="ingredient in ingredients" :key="ingredient.name"
           class="d-flex col-10 col-sm-9 col-md-6 col-lg-4 col-xl-3 mb-5">
        <div class="col-12 d-flex flex-column justify-content-start align-items-start">
          <div class="mb-4">
            <img :src="require('../../assets/images/index/flamelean-ingredients/' + ingredient.image)"
                 :alt="ingredient.name + ' image'"
                 width="115"
                 height="115"
                 class="d-flex justify-content-center"
            />
          </div>
          <div>
            <div class="fs-5 fw-bold mb-3 text-secondary">{{ ingredient.name }}</div>
            <ul class="list-unstyled">
              <li v-for="feature in ingredient.features" :key="feature" class="d-flex align-items-start mb-2">
                <img src="../../assets/images/index/check.svg"
                     alt="Check icon"
                     width="17" height="17"
                     class="me-2 mt-1"
                />
                <span class="text-secondary">{{ feature }}</span>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="d-flex justify-content-center text-center">
      <button class="btn btn-outline-primary px-5 py-2">See all ingredients</button>
    </div>
  </section>
</template>

<script>
export default {
  name: "FlameleanIngredientsSection",
  data() {
    return {
      ingredients: [
        {
          name: 'White Mullbery',
          image: 'white-mullbery.png',
          features: [
            `Used for centuries in Chinese
medicine to manage diabetes`,
            `Contains high levels of antioxidants
flavonoids`,
          ]
        },
        {
          name: 'Yarrow',
          image: 'yarrow.png',
          features: [
            `Used for centuries in traditional
medicine`,
            `Antioxidant and anti-inflammatory`,
            `Can significantly alleviate diarrhea`,
          ]
        },
        {
          name: 'Cayyene',
          image: 'cayyene.png',
          features: [
            `Can increase feelings of fullness`,
            `May have a positive impact on fat
oxidation`,
            `Helps optimize metabolic rate`,
          ]
        },
        {
          name: 'Vanadium',
          image: 'vanadium.png',
          features: [
            `Used for centuries in
traditional medicine`,
            `Antioxidant and
anti-inflammatory`,
            `Can significantly alleviate
diarrhea`,
          ]
        },
        {
          name: 'Manganese',
          image: 'manganese.png',
          features: [
            `Supports optimal bone formation`,
            `Keeps your nervous system in
check`,
            `Regulates carbohydrate and lipid
metabolism`,
            `Can help maintain blood glucose
levels`,
          ]
        },
        {
          name: 'Banaba',
          image: 'banaba.png',
          features: [
            `Can increase body heat production
and enhance weight loss`,
            `May have a positive effect on
blood sugar management`,
            `Helps lower blood glucose levels`,
            `Naturally mimicks action of insulin`,
          ]
        },
        {
          name: 'Guggul',
          image: 'guggul.png',
          features: [
            `Remedy used for centuries in
Ayurvedic medicine`,
            `Helps manage cholesterol levels`,
          ]
        },
        {
          name: 'Bitter Melon',
          image: 'bitter-melon.png',
          features: [
            `Long been a staple in
traditional medicine`,
            `Can significantly reduce
fasting blood sugar`,
            `May lower a long-term blood
sugar marker (HbA1c)`,
            `Helps decrease triglyceride
levels`,
          ]
        },
      ],
    }
  }
}
</script>

<style scoped>

</style>
