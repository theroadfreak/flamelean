<template>
  <div class="d-flex flex-column align-items-start fs-5 col-lg-9 mx-auto">
  <div class="px-0">
    <div v-for="(item, i) in orderedList" :key="i" class="mb-4">
       <div><b>{{item.title}}</b> {{item.text}}</div>
    </div>
  </div>
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
