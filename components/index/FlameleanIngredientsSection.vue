<template>
  <section class="container pt-5">
    <div class="d-flex flex-column justify-content-center align-items-center text-center text-secondary mb-5">
      <h2 class="fw-bold mb-5">Inside Every Flamelean capsule you’ll find</h2>
      <div class="col-12 col-md-8 col-xl-6 mb-md-5">
        6 clinically-proven ingredients that target inner body temperature
        <span class="fw-bold">supercharging</span> your calorie-burning engine
      </div>
    </div>
    <div class="row d-flex justify-content-center align-items-center">
      <div v-for="ingredient in ingredients" :key="ingredient.name" class="d-flex justify-content-center col-12 col-md-6 col-xl-5 mb-5">
        <div class="d-flex align-items-center align-items-lg-start">
          <div class="me-4">
            <img :src="require('../../assets/images/index/flamelean-ingredients/' + ingredient.image)"
                 :alt="ingredient.name + ' image'"
                 width="150"
                 height="150"
            />
          </div>
          <div>
            <div class="fs-5 fw-bold mb-3">{{ ingredient.name }}</div>
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
  </section>
</template>

<script>
export default {
  name: "FlameleanIngredientsSection",
  data() {
    return {
      ingredients: [
        {
          name: 'Perilla',
          image: 'ingredient-1.png',
          features: [
            'boosts BAT',
            'supports brain health',
            'supports healthy cholesterol',
          ]
        },
        {
          name: 'Perilla',
          image: 'ingredient-2.png',
          features: [
            'boosts BAT',
            'supports brain health',
            'supports healthy cholesterol',
          ]
        },
        {
          name: 'Perilla',
          image: 'ingredient-1.png',
          features: [
            'boosts BAT',
            'supports brain health',
            'supports healthy cholesterol',
          ]
        },
        {
          name: 'Perilla',
          image: 'ingredient-2.png',
          features: [
            'boosts BAT',
            'supports brain health',
            'supports healthy cholesterol',
          ]
        },
        {
          name: 'Perilla',
          image: 'ingredient-1.png',
          features: [
            'boosts BAT',
            'supports brain health',
            'supports healthy cholesterol',
          ]
        },
        {
          name: 'Perilla',
          image: 'ingredient-2.png',
          features: [
            'boosts BAT',
            'supports brain health',
            'supports healthy cholesterol',
          ]
        },
      ],
    }
  }
}
</script>

<style scoped>

</style>
