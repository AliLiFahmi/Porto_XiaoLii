<template>
  <div id="app">
    <div v-if="isLoad">
      <LoadingPage />
    </div>
    <div v-else>
      <HeaderPage />
      <HeroPage />
      <StatsPage />
      <DaftarPortoPage />
      <!-- <PortoPage /> -->
      <TheTimelinePage />
      <!-- <TimelinePage /> -->
      <FormPage />
      <FooterPage />
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";
import HeaderPage from "./components/HeaderPage.vue";
import HeroPage from "./components/HeroPage.vue";
import StatsPage from "./components/StatsPage.vue";
import DaftarPortoPage from "./components/DaftarPortoPage.vue";
// import PortoPage from "./components/PortoPage.vue";
import TheTimelinePage from "./components/TheTimelinePage.vue";
// import TimelinePage from "./components/TimelinePage.vue";
import FormPage from "./components/FormPage.vue";
import LoadingPage from "./components/LoadingPage.vue";
import FooterPage from "./components/FooterPage.vue";
const isLoad = ref(true);
onMounted(async () => {
  await simulateAsyncTask();

  isLoad.value = false;
});

async function simulateAsyncTask() {
  await new Promise((resolve) => setTimeout(resolve, 1500));
}
</script>
