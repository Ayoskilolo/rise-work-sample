<script setup lang="ts">
// import { RouterLink, RouterView } from 'vue-router'
import Header from './components/NavBar.vue';
import Footer from './components/FooterNav.vue'
import HeroSection from './views/HeroSection.vue'
import ServicesSection from './views/ServicesSection.vue'
import AssetClasses from './views/AssetSection.vue'
import StartSavingSection from './views/StartSavingSection.vue'
import RegulationSection from './views/RegulationSection.vue'
import CustomerReviewSection from './views/CustomersSection.vue'
import CommunitySection from './views/CommunitySection.vue'
import JoinUsSection from './views/JoinUsSection.vue'

</script>

<template>
  <Header />
  <HeroSection />
  <ServicesSection />
  <AssetClasses />
  <StartSavingSection />
  <RegulationSection />
  <CustomerReviewSection />
  <CommunitySection />
  <JoinUsSection />
  <Footer />
</template>

<style scoped></style>
