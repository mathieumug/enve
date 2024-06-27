<template>
  <div>
    <section id="projects" class="py-12 md:py-16 bg-blue-50">
      <div class="max-w-5xl mx-auto px-4 lg:px-10 relative">
        <div class="lg:py-3">
          <LineItem title="OUR PROJECTS" />
        </div>
        <div class="lg:pl-3 flex flex-col lg:flex-row lg:items-end">
          <h1
            class="flex lg:w-[50%] shrink-0 flex-col md:flex-row capitalize lg:flex-col text-4xl font-bold tracking-tightest leading-none"
          >
            <span class="text-black">Here Is What We </span>
            <span class="text-[#0071BC] md:pl-1.5 lg:pl-0">Have Worked On</span>
          </h1>
        </div>

        <div class="example pt-16">
          <swiper class="swiper" :options="swiperOption">
            <swiper-slide v-for="image in images" :key="image">
              <img class="w-full h-full object-cover" :src="image" alt="" />
            </swiper-slide>
          </swiper>
          <div class="text-black next">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              stroke="currentColor"
              stroke-width="1.5"
              class="size-12 bg-green-100 rounded-full p-3.5"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3"
              />
            </svg>
          </div>

          <div class="text-black prev">
            <svg
              fill="none"
              stroke="currentColor"
              stroke-width="1.5"
              class="size-12 bg-green-100 rounded-full p-3.5"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M10.5 19.5 3 12m0 0 7.5-7.5M3 12h18"
              />
            </svg>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import ProjectItem from "./Projects/ProjectItem.vue";
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

export default {
  components: {
    ProjectItem,
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      images: [
        "gallery/1.gif",
        "gallery/1.jpg",
        "gallery/2.webp",
        "gallery/3.webp",
        "gallery/4.webp",
        "gallery/5.webp",
        "gallery/6.webp",
        "images/project-2.jpg",
        "images/solar.webp",
      ],
      swiperOption: {
        slidesPerView: 2,
        centeredSlides: true,
        spaceBetween: 30,
        pagination: true,
        navigation: {
          nextEl: ".next",
          prevEl: ".prev",
        },
      },
    };
  },
};
</script>
<style scoped>
.swiper {
  width: 100%;
  height: 280px;
}
.swiper-slide {
  font-size: 18px;
  background: #ffffff;
  height: 270px;
  box-shadow: rgb(0 0 0 / 8%) 0px 1px 20px 0px;
}

.next,
.prev {
  position: absolute;
  top: 65%;
  z-index: 99;
}
.next {
  right: 25%;
}
.prev {
  left: 25%;
}
</style>
