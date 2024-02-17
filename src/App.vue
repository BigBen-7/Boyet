<template>
  <div id="app">
    <Navbar />
    <HeroSection />
    <ServicesSection />
    <LeadingSection />
    <MeetPeople />
    <CustomersReviews />
    <CaseStudySection />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import HeroSection from './components/HeroSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import LeadingSection from './components/LeadingSection.vue'
import MeetPeople from './components/MeetPeople.vue'
import CustomersReviews from './components/CustomersReviews.vue'
import CaseStudySection from './components/CaseStudySection.vue'

export default {
  components: {
    Navbar,
    HeroSection,
    ServicesSection,
    LeadingSection,
    MeetPeople,
    CustomersReviews,
    CaseStudySection
  }
}
</script>
