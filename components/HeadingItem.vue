<template>
  <h2 class="pt-2 pb-6 font-bold text-4xl text-tbs-deep-blue" :class="width">
    {{ heading }}
  </h2>
</template>

<script>
export default {
  props: {
    heading: String,
    width: String,
  },
};
</script>

<style></style>
