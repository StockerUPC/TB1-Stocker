<script setup>
import ClientSection from "@/components/ClientSection.vue";
import InventorySection from "@/components/InventorySection.vue";
import landingHeader from "@/components/LandingHeader.vue";
import principalSection from "@/components/PrincipalSection.vue";
import stockSection from "@/components/StockSection.vue";
import SupportPage from "@/components/SupportSection.vue";
import FooterSection from "@/components/FooterSection.vue";
</script>

<template>
    <landing-header/>
  <main>
    <div><principal-section/></div>
    <div><ClientSection/></div>
    <div><stock-section/></div>
    <div><InventorySection/></div>
    <div><SupportPage/></div>
    <div class="footer-section"><FooterSection/></div>
  </main>

</template>

<style scoped>
main{
  overflow: auto;
  position: relative;
  width: 100%;
  height: 100vh;
  scroll-snap-type: y var(--tw-scroll-snap-strictness);
  --tw-scroll-snap-strictness: mandatory;
}
div{
  scroll-snap-align: center;
}
</style>
