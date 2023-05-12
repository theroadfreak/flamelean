<template>
  <section class="row my-4 px-3 px-md-4">
    <div v-for="effect in sideEffects" class="col-12 col-md-6 d-flex justify-content-center mb-3">
      <div>
        <h2 v-html="effect.title"></h2>
        <ul>
          <li v-for="risk in effect.risks">{{ risk }}</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>

export default {
  name: "CommonSideEffectsSection",
  data() {
    return {
      sideEffects: [
        {
          title: `My Doctor Made Me Aware Of The<br class="d-none d-sm-flex" />
                    Common Side Effects, Like:`,
          risks: [
            'Nausea...',
            'Stomach Pain...',
            'Vomiting...',
            'And stomach pain...'
          ],
        },
        {
          title: `And Then The More Serious Risks, Like:`,
          risks: [
            'Kidney problems...',
            'Pancreatitis...',
            'Gallstones...',
            'Or severe allergic reactions'
          ],
        }
      ],
    }
  }
}
</script>

<style scoped>

</style>
