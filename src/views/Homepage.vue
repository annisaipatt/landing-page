<template>
  <TheNavbar></TheNavbar>
  <div class="relative">
    <TheBanner></TheBanner>
  </div>
  <div class="relative">
    <TheHome></TheHome>
  </div>
  <div class="relative">
    <TheServices></TheServices>
  </div>
</template>
<script setup>
import TheNavbar from "../components/TheNavbar.vue";
import TheBanner from "../components/TheBanner.vue";
import TheHome from "../components/TheHome.vue";
import TheServices from "@/components/TheServices.vue";
</script>
