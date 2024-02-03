<template>
  <div id="app">
    <Navbar />
    <HeroSection />
    <ServicesSection />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import HeroSection from './components/HeroSection.vue'
import ServicesSection from './components/ServicesSection.vue'
export default {
  components: {
    Navbar,
    HeroSection,
    ServicesSection
  }
}
</script>
