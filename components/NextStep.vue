<template>
  <div
    class="container py-5 d-flex justify-content-center text-center text-primary line-height-normal"
  >
    <a :href="link">
      Thanks, but no thanks Jessica. I understand this discount is a one-time
      special offer that’s only available right now.<br />
      But I’m going to stick with what I ordered. Please take me to the next
      step...
    </a>
  </div>
</template>

<script>
export default {
  name: "NextStep",
  props: {
    link: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped></style>
