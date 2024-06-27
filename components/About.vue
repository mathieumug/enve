<template>
  <div>
    <section
      id="about"
      class="pt-12 md:pt-0 bg-[#F0F9FF] overflow-hidden relative"
    >
      <div class="flex flex-col lg:flex-row">
        <div
          class="flex flex-col justify-center shrink-0 p-4 md:p-12 lg:p-0 lg:w-[50%] lg:pr-12 lg:pl-12 xl:pl-40 xl:pr-24"
        >
          <LineItem title="About Us" />
          <div class="md:pl-3">
            <h1
              class="flex md:flex-col py-3 text-4xl font-bold tracking-tightest leading-none"
            >
              <span class="text-black">Who</span>
              <span class="text-[#0071BC] pl-1.5 md:pl-0">We Are</span>
            </h1>
            <p
              class="text-sm lg:text-base text-left md:text-justify text-[#4C616F] py-2"
            >
              We are a private company limited by shares. The company has a
              number services to which includes but not limited to: act as
              Building and Construction, Solar and grid installations works,
              Water development and Construction of Motorized water systems,
              Services and general supplies etc. The Company has qualified and
              competent staff to render the services to our clients which is of
              high quality.
              <span class="font-bold"
                >ENVE ENGINEERING CONSULTS UG LIMITED</span
              >
              confirm that we are eligible to participate in the service
              delivery in Uganda. We undertake to abide by Code of Ethical
              Conduct for Bidders and Providers during the procurement process
              and the execution of any resulting contract:
            </p>
          </div>
        </div>
        <div class="flex-1 pb-[80%] md:pb-[45%] xl:pb-[50%] relative">
          <img
            src="images/img2.jpg"
            class="absolute h-full w-full object-cover"
            alt=""
          />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import LineItem from "./LineItem.vue";
import HeadingItem from "./HeadingItem.vue";
export default {
  components: {
    LineItem,
    HeadingItem,
  },
};
</script>
