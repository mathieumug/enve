<template>
  <div>
    <section id="contact">
      <div class="max-w-5xl md:py-20 mx-auto lg:px-0">
        <div class="flex flex-col lg:flex-row">
          <div
            class="flex flex-col px-5 py-16 lg:shrink-0 lg:pb-40 lg:pt-12 lg:pr-8 lg:w-[50%]"
          >
            <h1
              class="text-3xl pb-3 sm:pb-8 lg:text-4xl 2xl:text-5xl font-bold tracking-tighter"
            >
              Find us at
            </h1>

            <div class="lg:w-[75%]">
              <div class="flex items-center">
                <div
                  class="bg-[#d6efff] text-tbs-green w-[40px] h-[40px] lg:w-[50px] lg:lg:h-[50px] shrink-0 rounded-full flex justify-center items-center text-[#0D71BA]"
                >
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="w-5 h-5 lg:w-6 lg:h-6"
                  >
                    <path
                      fill-rule="evenodd"
                      d="m11.54 22.351.07.04.028.016a.76.76 0 0 0 .723 0l.028-.015.071-.041a16.975 16.975 0 0 0 1.144-.742 19.58 19.58 0 0 0 2.683-2.282c1.944-1.99 3.963-4.98 3.963-8.827a8.25 8.25 0 0 0-16.5 0c0 3.846 2.02 6.837 3.963 8.827a19.58 19.58 0 0 0 2.682 2.282 16.975 16.975 0 0 0 1.145.742zM12 13.5a3 3 0 1 0 0-6 3 3 0 0 0 0 6z"
                      clip-rule="evenodd"
                    />
                  </svg>
                </div>
                <div class="pl-4 py-4">
                  <p
                    class="leading-none text-sm lg:text-base w-full font-body text-slate-500"
                  >
                    We are located at Plot CH018 Church Road, off
                    Kyaliwajjala-Kira Road just after Total Fuel Station Uganda.
                  </p>
                </div>
              </div>
              <div class="flex items-center">
                <div
                  class="bg-[#d6efff] text-tbs-green w-[40px] h-[40px] lg:w-[50px] lg:h-[50px] shrink-0 rounded-full flex justify-center items-center text-[#0D71BA]"
                >
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="w-5 h-5 lg:w-6 lg:h-6"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M1.5 4.5a3 3 0 0 1 3-3h1.372c.86 0 1.61.586 1.819 1.42l1.105 4.423a1.875 1.875 0 0 1-.694 1.955l-1.293.97c-.135.101-.164.249-.126.352a11.285 11.285 0 0 0 6.697 6.697c.103.038.25.009.352-.126l.97-1.293a1.875 1.875 0 0 1 1.955-.694l4.423 1.105c.834.209 1.42.959 1.42 1.82V19.5a3 3 0 0 1-3 3h-2.25C8.552 22.5 1.5 15.448 1.5 6.75V4.5z"
                      clip-rule="evenodd"
                    />
                  </svg>
                </div>
                <div class="pl-4 py-4">
                  <span
                    class="text-sm lg:text-base font-body font-bold text-tbs-deep-blue"
                    >Call Us 24/7</span
                  >
                  <a
                    href="tel:+256394854329"
                    class="text-sm lg:text-base w-full font-body text-slate-500 leading-relaxed hover:underline hover:text-tbs-green block"
                    >+256 394 854 329
                  </a>
                  <a
                    href="tel:+256770953971"
                    class="text-sm lg:text-base w-full font-body text-slate-500 leading-relaxed hover:underline hover:text-tbs-green block"
                    >+256 770 953 971
                  </a>
                </div>
              </div>
              <div class="flex items-center">
                <div
                  class="bg-[#d6efff] text-tbs-green w-[40px] h-[40px] lg:w-[50px] lg:h-[50px] shrink-0 rounded-full flex justify-center items-center text-[#0D71BA]"
                >
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="w-5 h-5 lg:w-6 lg:h-6"
                  >
                    <path
                      d="M1.5 8.67v8.58a3 3 0 0 0 3 3h15a3 3 0 0 0 3-3V8.67l-8.928 5.493a3 3 0 0 1-3.144 0L1.5 8.67z"
                    />
                    <path
                      d="M22.5 6.908V6.75a3 3 0 0 0-3-3h-15a3 3 0 0 0-3 3v.158l9.714 5.978a1.5 1.5 0 0 0 1.572 0L22.5 6.908z"
                    />
                  </svg>
                </div>
                <div class="pl-4 py-4">
                  <span
                    class="text-sm lg:text-base font-body font-bold text-tbs-deep-blue"
                    >Mail Us</span
                  >
                  <a
                    href="mailto:info@enveengineeringconsultsug.org"
                    class="text-sm lg:text-base w-full font-body text-slate-500 leading-relaxed hover:underline hover:text-tbs-green block"
                    >info@enveengineeringconsultsug.org
                  </a>
                </div>
              </div>
            </div>
          </div>

          <div class="lg:flex-1 h-full bg-red-100">
            <Map />
          </div>
        </div>
      </div>
      <div class="h-[60px] bg-[#0071BC] justify-center flex items-center">
        <h1
          class="font-semibold text-white text-center px-4 text-[12px] lg:text-base"
        >
          Copyright &copy;
          <span id="copyright">
            <script>
              document
                .getElementById("copyright")
                .appendChild(document.createTextNode(new Date().getFullYear()));
            </script>
          </span>
          Enve Engineering Consults (Ug) Ltd. All rights reserved.
        </h1>
      </div>
    </section>
  </div>
</template>

<script>
import Map from "./Map.vue";

export default {
  components: {
    Map,
  },
};
</script>
