<template>
  <div class="bg-secondary pt-20 pb-16">
    <div class="container mx-auto">
      <div class="mb-14 px-2 text-center">
        <h1
          data-aos="fade-left"
          data-aos-delay="500"
          data-aos-duration="1000"
          data-aos-offset="720"
          class="text-ghost text-3xl mb-4 md:text-4xl 2xl:text-5xl font-bold font-nunitosans"
        >
          My Experience
        </h1>
        <p
          data-aos="fade-left"
          data-aos-delay="800"
          data-aos-duration="1000"
          data-aos-offset="730"
          class="text-lg 2xl:text-xl text-ghost font-pops"
        >
          This is some of my experience during my time in the web development
          field.
        </p>
      </div>
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
    <img
      :src="circle"
      data-aos="fade-right"
      data-aos-delay="700"
      data-aos-offset="730"
      data-aos-duration="1000"
      data-aos-easing="ease-in-out"
      alt="circle"
      class="relative pl-4 mt-14 md:pl-6 md:scale-150 scale-110"
    />
  </div>
</template>

<script setup>
import circle from "../assets/circle.svg";

</script>
