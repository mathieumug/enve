<template>
  <div class="pb-[50%] md:pb-[25%] relative">
    <div class="z-[10] absolute top-0 size-full bgrad">
      <div class="flex items-center size-full max-w-5xl mx-auto text-white">
        <div>
          <h1
            class="font-bold leading-none text-2xl md:text-4xl xl:text-5xl w-[80%] mx-auto text-center xl:text-left xl:mx-0"
          >
            Leading engineering services & solutions consultancy in Uganda
          </h1>

          <div class="mx-auto xl:mx-0 w-[280px] md:w-[320px] my-5">
            <a
              class="bg-white flex justify-between items-center font-semibold text-[#0071BC] cursor-pointer hover:bg-opacity-80 text-sm md:text-base rounded py-2 md:py-3 xl:py-3.5 px-5"
              href="#contact"
            >
              <span class="capitalize">Book your consultancy now</span>
              <span class="text-[#0071BC]">
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
        </div>
      </div>
    </div>
    <img
      src="images/banner.jpg"
      class="absolute size-full object-cover"
      alt=""
    />
  </div>
</template>

<script>
export default {};
</script>

<style>
.bgrad {
  background: linear-gradient(90deg, #ff0000 5%, transparent 130%);
}
</style>
