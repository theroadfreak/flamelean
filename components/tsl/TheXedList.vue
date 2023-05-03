<template>
  <section class="container d-flex flex-column align-content-center text-center fs-5">
    <div v-for="(li, i) in list" :key="i" class="mb-3">
      <img src="../../assets/images/tsl/common-side-effects-section/x-icon.svg" alt="X icon"><span>{{li}}</span>
    </div>
  </section>
</template>

<script>
export default {
  name: "TheXedList",
  props: {
    list: {
      type: Object,
      default: []
    }
  }
}
</script>

<style scoped>

</style>
