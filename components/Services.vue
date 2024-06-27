<template>
  <section id="services" class="py-12 md:py-24">
    <div class="max-w-5xl mx-auto px-4 lg:px-10">
      <div class="lg:py-3">
        <LineItem title="Our Services" />
      </div>
      <div class="lg:pl-3 flex flex-col lg:flex-row lg:items-end">
        <h1
          class="flex lg:w-[30%] shrink-0 lg:flex-col text-4xl font-bold tracking-tightest leading-none"
        >
          <span class="text-black">Here is </span>
          <span class="text-[#0071BC] pl-1.5 lg:pl-0">What we do</span>
        </h1>
        <div class="flex-1">
          <p
            class="py-2 lg:py-0 font-xl leading-tight tracking-tight text-black font-semibold"
          >
            We are an Engineering firm that focuses on projects like general
            construction, water development works, irrigation systems,
            consultancy services, extra
          </p>
        </div>
      </div>

      <div class="pt-6 xl:pt-16">
        <ServiceItem
          title="Motorized Solar Water pumping"
          body="We implement, on behalf of our clients, Solar powered water supply schemes in rural communities and institutions to provide access to clean water. This technology combines solar panels, which convert sunlight into electricity, with a motorized pump to draw and transport water for various purposes such as irrigation, livestock, or domestic use."
          image="images/img2.jpg"
          bgColorOrder="bg-white"
        />

        <ServiceItem
          title="Rain Water Harvesting"
          body="This in institutions like schools, health centers, we harvest this kind of water and keep it into either a rasied or undergorund storage, thereafter distributed to various collection points for different use cases."
          image="images/rain-water.jpg"
          bgColorOrder="bg-white lg:flex-row-reverse"
        />

        <ServiceItem
          title="Construction and Rehabilitation of Water sources"
          body="Construction and Rehabilitation of Water sources - We construct and also carry out rehabilitaion of water sources like boreholes and protected water springs, in spacely populated places to continue access to clean water to communities."
          image="gallery/3.webp"
          bgColorOrder="bg-white"
        />

        <ServiceItem
          title="Irrigation Projects"
          body="A solar irrigation project involves the implementation of solar-powered systems to enhance and optimize the process of irrigating agricultural fields.By utilizing solar energy through photovoltaic panels, these projects aim to provide a sustainable and environmentally friendly solution to power irrigation pumps."
          image="images/img3.jpg"
          bgColorOrder="bg-white lg:flex-row-reverse"
        />

        <ServiceItem
          title="Sanitary construction"
          body="We have constructed a number of VIP latrines on behalf of our clients to continue to implement clean hygiene to the communities in Uganda. We work hand-in-hand with different clients to continue to advocate for proper hygiene as we implement these projects on their behalf."
          image="images/img5.jpg"
          bgColorOrder="bg-white"
        />

        <ServiceItem
          title="General construction"
          body="Our team of Engineers is dedicated to bringing you the best quality in your construction needs, be it putting up new structure or renovating the existing ones, we are committed to delivering the same high quality within the allocated time frame. We handle projects like classroom blocks, health centers, commercial buildings, extra."
          image="images/img4.jpg"
          bgColorOrder="bg-white lg:flex-row-reverse"
        />
      </div>
    </div>
  </section>
</template>

<script>
import ServiceItem from "./ServiceItem.vue";
import MoreServices from "./MoreServices.vue";

export default {
  components: {
    ServiceItem,
    MoreServices,
  },
};
</script>
