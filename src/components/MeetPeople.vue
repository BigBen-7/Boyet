<template>
  <section class="meet-people-section">
    <div class="container mx-auto">
      <!-- Section Heading -->
      <div class="meet-people-heading mb-10">
        <LineReuseable />

        <h2 class="text-3xl">Meet The people <span class="meet">We are working with</span></h2>
      </div>

      <!-- Image Logos -->
      <div class="logos-container flex justify-center w-full p-10 bg-gray-100 m-10">
        <!-- Loop through image URLs and display them -->
        <div
          v-for="(image, index) in imageUrls"
          :key="index"
          class="rounded-lg overflow-hidden logos"
        >
          <img :src="image" alt="logos" class="w-18 h-auto" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import LineReuseable from './LineReuseable.vue'
// import LineReuseable from './LineReuseable.vue'
export default {
  name: 'MeetPeople',
  components: {
    LineReuseable
  },
  data() {
    return {
      // Example image URLs, replace with your actual image URLs
      imageUrls: [
        '/src/assets/logos/Logo-7.png',
        '/src/assets/logos/Logo-9.png',
        '/src/assets/logos/Logo5.png',
        '/src/assets/logos/Logo8.png',
        '/src/assets/logos/Logo9.png',
        '/src/assets/logos/Logo-6.png'
      ]
    }
  }
}
</script>

<style scoped>
@import '../styles/meet.css'; /* Add scoped styles if needed */
</style>
