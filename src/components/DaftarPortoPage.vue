<template>
  <div>
    <div
      data-aos="fade-right"
      data-aos-delay="300"
      data-aos-duration="1000"
      data-aos-offset="400"
    >
      <img
        :src="dot1"
        alt="dot"
        class="xl:scale-[.61] 2xl:-top-24 relative -top-24 xl:-top-16 scale-50 -ml-5 xl:-ml-2"
      />
    </div>
    <div
      data-aos="fade-left"
      data-aos-delay="300"
      data-aos-duration="1000"
      data-aos-offset="400"
    >
      <img
        :src="circle"
        alt="circle"
        class="ml-auto scale-110 md:scale-150 relative -top-52 pr-5 md:pr-10 lg:pr-8 2xl:pr-14"
      />
    </div>
    <img
      data-aos="fade-left"
      data-aos-delay="300"
      data-aos-duration="500"
      :src="dashcircle"
      alt="dashcircle"
      class="absolute -right-20 hidden md:block -bottom-[60rem] lg:-bottom-[65rem] 2xl:-bottom-[70rem] 2xl:scale-150"
    />
  </div>
  <div
    data-aos="fade-up"
    data-aos-delay="300"
    data-aos-offset="570"
    data-aos-duration="800"
    id="portfolio"
    class="pb-10 -mt-28 xl:-mt-5 2xl:-mt-36"
  >
    <div class="container mx-auto 2xl:mt-14">
      <div
        class="flex-col md:flex-row lg:flex items-center xl:px-10 2xl:px-14 justify-between mb-14 lg:mb-0"
      >
        <div class="text-center lg:text-left px-5 xl:px-0 mb-12">
          <h1
            data-aos="fade-up"
            data-aos-delay="500"
            data-aos-duration="1000"
            data-aos-offset="650"
            class="text-3xl font-bold mb-4 md:text-4xl 2xl:text-5xl text-ghost font-nunitosans"
          >
            Projects
          </h1>
          <p
            data-aos="fade-up"
            data-aos-delay="500"
            data-aos-duration="1000"
            data-aos-offset="650"
            class="text-ghost text-lg 2xl:text-xl text-center leading-relaxed lg:text-left lg:max-w-lg font-pops"
          >
            This is some work that I have created to share and showcase what I
            have accomplished so far.
          </p>
        </div>
      </div>
      <!-- projects -->
      <div
        data-aos="fade-up"
        data-aos-delay="600"
        data-aos-duration="1000"
        data-aos-offset="550"
        data-aos-easing="ease-in-out"
        class="flex flex-wrap px-5 xl:px-10 2xl:px-12 items-center justify-center mb-8"
      >
        <span
          class="text-ghost text-lg 2xl:text-xl text-center leading-relaxed lg:text-left lg:max-w-lg font-pops"
        >
          Not Data
        </span>
      </div>
    </div>
  </div>
</template>

<script setup>
import dot1 from "../assets/dot.png";
import circle from "../assets/circle.svg";
import dashcircle from "../assets/dashcircle.svg";
import { ref, computed } from "vue";
const itemsPerPage = 3;
const currentPage = ref(0);

const displayedItems = computed(() => {
  const startIndex = currentPage.value * itemsPerPage;
  const endIndex = startIndex + itemsPerPage;
  return items.value.slice(startIndex, endIndex);
});

const totalPageCount = computed(() =>
  Math.ceil(items.value.length / itemsPerPage)
);

</script>
