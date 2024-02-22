<template>
  <TheNavbar></TheNavbar>
  <div class="relative">
    <TheBanner></TheBanner>
  </div>
  <div class="relative">
    <TheHome></TheHome>
  </div>
  <div class="relative">
    <ToolsTechnology></ToolsTechnology>
  </div>
  <div class="relative">
    <ToolsTechnology></ToolsTechnology>
  </div>
  <div class="relative">
    <OurPricing></OurPricing>
  </div>
</template>
<script setup>
import TheNavbar from "../components/TheNavbar.vue";
import TheBanner from "../components/TheBanner.vue";
import TheHome from "../components/TheHome.vue";
import ToolsTechnology from "@/components/ToolsTechnology.vue";
import OurPricing from "@/components/OurPricing.vue";
</script>
