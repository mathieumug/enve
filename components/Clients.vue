<template>
  <div>
    <section id="clients" class="py-12 md:py-24">
      <div class="max-w-5xl mx-auto px-4 lg:px-10">
        <div class="lg:py-3">
          <LineItem title="Our Clients" />
        </div>
        <div class="lg:pl-3 flex flex-col lg:flex-row lg:items-end">
          <h1
            class="flex lg:w-[50%] shrink-0 flex-col md:flex-row capitalize lg:flex-col text-4xl font-bold tracking-tightest leading-none"
          >
            <span class="text-black">Our Happy</span>
            <span class="text-[#0071BC] md:pl-1.5 lg:pl-0">Clients</span>
          </h1>
        </div>

        <div
          class="py-6 md:py-12 grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4"
        >
          <LogoItem url="logos/1.jpg" size="w-16 bg-[#F5F5F5]" />
          <LogoItem url="logos/2.png" size="w-40 bg-[#F5F5F5]" />
          <LogoItem url="logos/3.png" size="w-40 bg-[#F5F5F5]" />
          <LogoItem url="logos/4.png" size="w-16 bg-[#F5F5F5]" />
          <LogoItem url="logos/5.png" size="w-40 bg-[#F5F5F5]" />
          <LogoItem url="logos/6.png" size="w-40 bg-[#F5F5F5]" />
          <LogoItem url="logos/7.png" size="w-20 bg-[#F5F5F5]" />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import LogoItem from "./LogoItem.vue";
export default {
  components: {
    LogoItem,
  },
};
</script>
