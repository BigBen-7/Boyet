<template>
  <div id="app">
    <Navbar />
    <ServicesPage />
    <!-- <HeroSection />
    <ServicesSection />
    <LeadingSection />
    <MeetPeople />
    <CustomersReviews />
    <CaseStudySection /> -->
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import ServicesPage from './Pages/ServicesPage.vue'
// import HeroSection from './components/HeroSection.vue'
// import ServicesSection from './components/ServicesSection.vue'
// import LeadingSection from './components/LeadingSection.vue'
// import MeetPeople from './components/MeetPeople.vue'
// import CustomersReviews from './components/CustomersReviews.vue'
// import CaseStudySection from './components/CaseStudySection.vue'

export default {
  components: {
    Navbar,
    ServicesPage
  }
}
</script>
