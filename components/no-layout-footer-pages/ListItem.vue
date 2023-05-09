<template>
  <div class="d-flex flex-column align-items-start fs-5 col-lg-9 mx-auto">
  <ol>
    <li v-for="(item, i) in orderedList" :key="i" class="mb-4">
       <div v-html="item"></div>
    </li>
  </ol>
</div>
</template>

<script>
export default {
  name: "ListItem",
  props: {
    orderedList:{
      type: Array,
      default: []
    }
  }
}
</script>

<style scoped>

</style>
