<template>
  <section class="bg-primary">
    <div class="container d-flex flex-column align-items-center py-5">
      <h2 class="fw-bold text-center text-white mb-5">Frequently Asked Questions</h2>
      <div class="col-11 col-sm-12 col-lg-11 col-xl-10">
        <div class="accordion accordion-flush bg-transparent w-100" id="accordionFAQ">
          <div v-for="(accordionItem, i) in accordionItems"
               class="accordion-item w-100 rounded rounded-3"
               :class="{ 'mb-3' : i !== accordionItems.length - 1 }"
          >
            <h2 class="accordion-header" :id="'heading_' + i">
              <button
                class="accordion-button rounded rounded-3 bg-white border border-0 collapsed text-secondary fw-bold"
                type="button"
                data-bs-toggle="collapse"
                :data-bs-target="'#collapse_' + i"
                aria-expanded="false"
                :aria-controls="'#collapse_' + i"
              >
                <span class="py-1">{{ accordionItem.question }}</span>
              </button>
            </h2>
            <div :id="'collapse_' + i" class="accordion-collapse collapse" :aria-labelledby="'heading_' + i"
                 data-bs-parent="#accordionFAQ">
              <div class="accordion-body col-12 col-lg-10 col-xl-9 pt-0 pb-4">
                {{ accordionItem.answer }}
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "FrequentlyAskedQuestionsSection",
  data() {
    return {
      accordionItems: [
        {
          question: 'Is Flamelean right for me?',
          answer: 'We promise your money back if the item you received is not as described,\n' +
            'or if your item is not delivered within the Buyer Protection period.',
        },
        {
          question: 'Is Flamelean safe?',
          answer: 'We promise your money back if the item you received is not as described,\n' +
            'or if your item is not delivered within the Buyer Protection period.',
        },
        {
          question: 'Is Flamelean right for me?',
          answer: 'We promise your money back if the item you received is not as described,\n' +
            'or if your item is not delivered within the Buyer Protection period.',
        },
      ]
    }
  }
}
</script>

<style scoped>

</style>
