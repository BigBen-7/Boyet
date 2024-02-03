<template>
  <section class="services-section">
    <div class="container mx-auto">
      <!-- Service Header  -->
      <div class="services-header text-center">
        <h2 class="text-3xl font-bold">Service we offer</h2>
      </div>
    </div>
    <!-- Flex Container for Cards -->
    <div class="flex justify-evenly m-2 p-2">
      <!-- Cards -->
      <div v-for="(item, index) in swiperTextBase" :key="index" class="card mb-8">
        <div class="card-content">
          <h3 class="text-left font-bold mb-2 card-head">{{ item.heading }}</h3>
          <p class="text-black card-detail">{{ item.text }}</p>
        </div>
      </div>
    </div>
    <!-- </div> -->
  </section>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    const swiperTextBase = ref([
      {
        heading: 'Mobile App Development',
        text: 'A Website is an extension of yourself and we can help you to express it properly. Your website is your number one marketing asset because we live in a digital age.',
        image: ''
      },
      {
        heading: 'Web Design & Development',
        text: 'A Website is an extension of yourself and we can help you to express it properly. Your website is your number one marketing asset because we live in a digital age.',
        image: ''
      },
      {
        heading: 'Software Testing Service',
        text: 'A Website is an extension of yourself and we can help you to express it properly. Your website is your number one marketing asset because we live in a digital age.',
        image: ''
      }
    ])

    return { swiperTextBase }
  }
}
</script>

<style scoped>
@import '../styles/services.css';
</style>
