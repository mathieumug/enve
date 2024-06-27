<template>
  <div
    class="my-4 flex flex-col flex-col-reverse lg:flex-row"
    :class="bgColorOrder"
  >
    <div class="lg:w-[55%] px-4 py-8 sm:p-12 md:p-24">
      <h1 class="text-2xl tracking-tight text-black font-bold">
        {{ title }}
      </h1>
      <p class="text-[#4C616F] text-base py-2">
        {{ body }}
      </p>
    </div>

    <div class="flex-1 pb-[100%] sm:pb-[50%] lg:pb-[30%] relative">
      <img :src="image" class="absolute h-full w-full object-cover" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    body: String,
    image: String,
    style: String,
    bgColorOrder: String,
  },
};
</script>
