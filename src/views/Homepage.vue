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
  <div class="relative">
    <ToolsTechnology></ToolsTechnology>
  </div>
  <div class="relative">
    <OurPricing></OurPricing>
  </div>
  <div class="relative">
    <OurSpeciality></OurSpeciality>
  </div>
  <div class="relative">
    <TheTestimonial></TheTestimonial>
  </div>
  <div class="relative">
    <ContactUs></ContactUs>
  </div>
  <div class="relative">
    <TheFooter></TheFooter>
  </div>
</template>
<script setup>
import TheNavbar from "../components/TheNavbar.vue";
import TheBanner from "../components/TheBanner.vue";
import TheHome from "../components/TheHome.vue";
import ToolsTechnology from "@/components/ToolsTechnology.vue";
import OurPricing from "@/components/OurPricing.vue";
import OurSpeciality from "@/components/OurSpeciality.vue";
import TheServices from "@/components/TheServices.vue";
import TheTestimonial from "@/components/TheTestimonial.vue";
import ContactUs from "../components/ContactUs.vue";
import TheFooter from "../components/TheFooter.vue";
import "@fortawesome/fontawesome-free/css/all.css"
</script>
