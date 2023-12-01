<template>
  <div class="bg-secondary pt-20 pb-16">
    <div class="container mx-auto">
      <div class="mb-14 px-2 text-center">
        <h1
          class="text-ghost text-3xl mb-4 md:text-4xl 2xl:text-5xl font-bold font-nunitosans"
        >
          My Experience
        </h1>
        <progress
          class="text-lg 2xl:text-xl text-ghost font-pops"
        >
          This is some of my experience during my time in the web development
          field.
        </progress>
      </div>
      <div
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
      alt="circle"
      class="relative pl-4 mt-14 md:pl-6 md:scale-150 scale-110"
    />
  </div>
</template>

<script setup>
import circle from "../assets/circle.svg";

</script>
