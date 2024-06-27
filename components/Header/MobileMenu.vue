<template>
  <div>
    <header class="bg-white min-h-[60px]">
      <nav
        class="flex flex-row-reverse lg:flex-row items-center justify-between px-4 sm:px-6 lg:px-4"
        aria-label="Top"
      >
        <!-- Menu Icon -->
        <div
          @click="toggleMenu"
          class="xl:hidden lg:text-[#06071C] w-[52px] h-[52px] hover:bg-slate-200 cursor-pointer rounded-full flex items-center justify-center"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-7 h-7"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
            />
          </svg>
        </div>

        <!-- Logo -->
        <a href="">
          <Logo class="w-40" />
        </a>

        <!-- Call to action -->
        <div class="hidden lg:block">
          <a
            class="bg-[#0071BC] text-white cursor-pointer hover:bg-opacity-70 font-body font-semibold text-sm rounded-md text-[#06071C] py-2 px-5"
            href=""
            >Contact Us
          </a>
        </div>
      </nav>
    </header>

    <div
      :class="
        menuOpen ? 'translate-x-0' : 'translate-x-full lg:-translate-x-full'
      "
      class="z-[9999] bg-white fixed p-cst inset-y-0 left-0 md:left-[50%] right-0 lg:left-[0px] lg:right-[60%] flex flex-col overflow-y-hidden"
    >
      <div class="overflow-y-auto flex flex-col pb-8 pt-32 relative">
        <!-- Close Menu Button -->
        <div
          @click="toggleMenu"
          class="absolute top-[30px] right-[30px] hover:bg-gray-300 bg-gray-100 text-tbs-deep-blue rounded-full w-12 h-12 p-2 flex justify-center cursor-pointer items-center"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M6 18 18 6M6 6l12 12"
            />
          </svg>
        </div>

        <a
          @click="toggleMenu"
          v-for="link in navigation"
          :key="link.name"
          :href="link.href"
          class="font-body font-semibold text-[18px] text-tbs-blue py-2 px-8 my-2 hover:bg-slate-100"
          >{{ link.name }}</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menuOpen: false,
      navigation: [
        { name: "About", href: "#about" },
        { name: "Services", href: "#services" },
        { name: "Our Projects", href: "#projects" },
        { name: "Why Us", href: "#why" },
        { name: "Our Clients", href: "#clients" },
      ],
    };
  },

  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen;
    },
  },
};
</script>

<style>
.p-cst {
  transition: transform 250ms ease-in-out;
}
</style>
