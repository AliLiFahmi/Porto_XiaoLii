<template>
  <div class="bg-secondary pt-20 pb-16">
    <div class="container mx-auto">
      <div class="mb-14 px-2 text-center">
        <h1
          class="text-ghost text-3xl mb-4 md:text-4xl 2xl:text-5xl font-bold font-nunitosans"
        >
          My Experience
        </h1>
        <p
          class="text-lg 2xl:text-xl text-ghost font-pops"
        >
          This is some of my experience during my time in the web development
          field.
        </p>
      </div>
      <ol class="items-center px-6 md:px-10 lg:flex font-pops justify-center">
        <li
          v-for="(project, index) in projects"
          :key="index"
          class="relative mb-6"
        >
          <div class="flex items-center">
            <div
              class="z-10 flex items-center justify-center w-6 xs:w-8 h-6 xs:h-8 md:w-10 md:h-10 2xl:w-12 2xl:h-12 bg-redcake rounded-full shrink-0"
            >
              <i
                class="fa-solid fa-briefcase text-xs xs:text-sm md:text-lg 2xl:text-xl text-ghost"
              ></i>
            </div>
            <div
              class="sm:flex w-full bg-[#433D5A] h-0.5"
            ></div>
          </div>
          <div
            class="mt-3 sm:pr-8"
          >
            <h3 class="text-lg font-bold text-redcake md:text-xl xl:text-2xl">
              {{ project.title }}
            </h3>
            <time
              class="block mb-4 text-base md:text-lg font-semibold text-ghost"
              >{{ project.date }}</time
            >
            <p class="text-base 2xl:leading-loose text-ghost">
              {{ project.description }}
            </p>
          </div>
        </li>
      </ol>
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
const projects = [
  {
    title: "Freelance",
    date: "March 2020",
    description:
      "I have experience working as a freelance web developer where I assist clients in transforming their designs from Figma into fully functional websites. This experience has taught me the importance of precision and patience in achieving stunning designs.",
  },
  {
    title: "Freelance",
    date: "December 2020",
    description:
      "I have experience working as a freelance web developer where I assist clients in transforming their designs from Figma into fully functional websites. This experience has taught me the importance of precision and patience in achieving stunning designs.",
  },
  {
    title: "Cv. Semangat Mandiri",
    date: "April 2021",
    description:
      "Currently, I am working as an intern in an independent business owned by my father. In this role, I have been involved in various projects, including creating landing pages for different purposes and developing features within them.",
  },
];
</script>
