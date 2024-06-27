<template>
  <div>
    <section id="gallery" class="py-12 md:py-24">
      <div class="max-w-5xl mx-auto px-4 lg:px-10 relative">
        <div class="lg:py-3">
          <LineItem title="Our Projects" />
        </div>
        <div class="lg:pl-3 flex flex-col lg:flex-row lg:items-end">
          <h1
            class="flex lg:w-[50%] shrink-0 flex-col md:flex-row capitalize lg:flex-col text-4xl font-bold tracking-tightest leading-none"
          >
            <span class="text-black">Here is What we </span>
            <span class="text-[#0071BC] md:pl-1.5 lg:pl-0">have worked on</span>
          </h1>
        </div>

        <div class="example pt-16">
          <swiper class="swiper" :options="swiperOption">
            <swiper-slide>
              <ProjectItem
                title="Solar energy"
                body="Solar water pumping project carried out at Rhino camp in Arua District."
                url="images/solar.webp"
              />
            </swiper-slide>
            <swiper-slide>
              <ProjectItem
                title="Boreholes and clean water"
                body="Project Beneficiaries accessing clean water at Bidibidi Refuge Settlement camp - Yumbe District."
                url="images/project-2.jpg"
              />
            </swiper-slide>
            <swiper-slide>
              <ProjectItem
                title="Building and infrastructure"
                body="Construction of VIP Latrines."
                url="images/project-3.jpg"
              />
            </swiper-slide>
          </swiper>
          <div class="text-black next">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              stroke="currentColor"
              stroke-width="1.5"
              class="size-12 bg-red-100 rounded-full p-3.5"
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
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              stroke="currentColor"
              stroke-width="1.5"
              class="size-12 bg-red-100 rounded-full p-3.5"
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
      swiperOption: {
        slidesPerView: 3,
        centeredSlides: false,
        spaceBetween: 20,

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
  height: 380px;
}
.swiper-slide {
  font-size: 18px;
  background: #ffffff;
  height: 370px;
  box-shadow: rgb(0 0 0 / 8%) 0px 1px 20px 0px;
}

.next,
.prev {
  position: absolute;
  top: 55%;
  z-index: 99;
}
.next {
  right: 10px;
}
.prev {
  left: 10px;
}
</style>
