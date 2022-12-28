<template>
  <div class="flex flex-col min-h-screen font-Roboto bg-weather-primary h-max">
    <SiteNavigation />
    <RouterView />
  </div>
</template>

<script setup>
import { RouterView } from "vue-router";
import SiteNavigation from "./components/SiteNavigation.vue";
</script>

<style src="./assets/tailwind.css"></style>