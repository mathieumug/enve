<template>
  <div class="relative">
    <div
      class="absolute h-screen md:h-[600px] w-full z-[99] bg-trs flex flex-col"
    >
      <div class="w-full">
        <DesktopMenu class="hidden xl:block" />
        <MobileMenu class="xl:hidden" />
      </div>

      <div
        class="pb-10 md:pb-0 px-4 md:px-8 xl:px-0 xl:max-w-5xl xl:mx-auto flex items-end md:items-center flex-1"
      >
        <div
          class="text-left md:text-center xl:text-left mx-auto lg:w-[60%] xl:mx-0 xl:w-[60%]"
        >
          <h1
            class="text-[48px] md:text-[44px] leading-none tracking-tight font-bold text-white"
          >
            We deliver reliable, high quality and affordable engineering
            projects
          </h1>
          <p class="text-sm opacity-75 py-3 text-white leading-tight">
            We handle all sorts of engineering projects from irrigation
            projects, Motorized Solar Water Pumping, General construction,
            Sanitary construction and so many others.
          </p>

          <div class="md:mx-auto xl:mx-0 md:w-[300px] my-4">
            <a
              class="bg-[#0071BC] flex justify-between items-center font-semibold text-white cursor-pointer hover:bg-opacity-70 text-sm rounded text-[#06071C] py-3.5 md:py-2.5 px-5"
              href="#contact"
            >
              <span class="capitalize">Lets handle your project now</span>
              <span class="text-white">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="1.5"
                  class="size-6"
                  viewBox="0 0 24 24"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="m12.75 15 3-3m0 0-3-3m3 3h-7.5M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  />
                </svg>
              </span>
            </a>
          </div>

          <div
            class="mt-5 md:mt-10 flex flex-col md:flex-row items-center justify-center xl:justify-start"
          >
            <span class="text-[12px] mr-3 font-semibold text-white"
              >Trusted By:</span
            >
            <img src="/logos.png" class="w-[32rem]" alt="" />
          </div>
        </div>
      </div>
    </div>
    <swiper class="h-screen md:h-[600px] w-full" :options="swiperOption">
      <swiper-slide class="bg-[url('/slider/6.webp')]"></swiper-slide>
      <swiper-slide class="bg-[url('/slider/1.webp')]"></swiper-slide>
      <swiper-slide class="bg-[url('/slider/2.webp')]"></swiper-slide>
      <swiper-slide class="bg-[url('/slider/3.webp')]"></swiper-slide>
      <swiper-slide class="bg-[url('/slider/4.webp')]"></swiper-slide>
      <swiper-slide class="bg-[url('/slider/5.webp')]"></swiper-slide>
      <swiper-slide class="bg-[url('/slider/bg.jpg')]"></swiper-slide>
      <div
        class="swiper-pagination swiper-pagination-white"
        slot="pagination"
      ></div>
    </swiper>
  </div>
</template>

<script>
import DesktopMenu from "./Header/DesktopMenu.vue";
import MobileMenu from "./Header/MobileMenu.vue";

import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

export default {
  components: {
    DesktopMenu,
    MobileMenu,
    Swiper,
    SwiperSlide,
  },

  data() {
    return {
      swiperOption: {
        spaceBetween: 30,
        initialSlide: 0,
        autoplay: {
          delay: 1500,
          disableOnInteraction: true,
        },
        speed: 1000,
        effect: "fade",
        grabCursor: true,
        pagination: {
          el: ".swiper-pagination",
          clickable: true,
        },
      },
    };
  },
};
</script>

<style scoped>
.swiper {
  height: 360px;
}

.swiper-slide {
  background-position: center;
  background-size: cover;
}

.bg-trs {
  background: linear-gradient(360deg, #090e1e 8%, transparent 130%);
}
</style>
