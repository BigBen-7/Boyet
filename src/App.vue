<template>
  <div id="app">
    <Navbar />
    <HeroSection />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import HeroSection from './components/HeroSection.vue'
export default {
  components: {
    Navbar,
    HeroSection
  }
}
</script>
