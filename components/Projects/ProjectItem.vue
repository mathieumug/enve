<template>
  <div class="">
    <div class="pb-[80%] relative">
      <img :src="url" class="absolute size-full object-cover" alt="" />
    </div>
    <div class="py-2 px-4">
      <h1 class="text-[#0071BC] text-lg font-bold tracking-tight">
        {{ title }}
      </h1>
      <p class="text-[#4C616F] text-sm pb-4 leading-tight">
        {{ body }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    url: String,
    title: String,
    body: String,
  },
};
</script>
