<template>
  <div class="flex size-full items-center p-4 bg-[#F5F5F5]">
    <img :src="url" class="mx-auto" :class="size" alt="" />
  </div>
</template>

<script>
export default {
  props: {
    size: String,
    url: String,
  },
};
</script>
