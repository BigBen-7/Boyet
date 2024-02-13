<template>
  <div class="leading-section flex items-center justify-center my-60">
    <!-- Text and image container  -->
    <div class="container mx-auto flex flex-col lg:flex-row items-center justify-center">
      <!-- Text Content  -->
      <div class="text-content lg:w-1/2 lg:pr-8">
        <LineReuseable />
        <h2 class="text-3xl font-medium mb-4 leading-head">
          Leading companies trust us <span class="develop">to develop software </span>
        </h2>
        <p class="text-gray-700 mb-8 content">
          We <span class="add"> add development capacity </span>
          to tech teams. Our value isn’t limited to building teams but is equally distributed across
          the project lifecycle. We are a custom software development company that guarantees the
          successful delivery of your project.
        </p>
        <!-- Button with Arrow Icon -->
        <button class="flex items-center lead-btn">See more Information</button>
      </div>
      <!-- Image -->
      <div class="image-container lg:w-1/2 lg:pl-8">
        <img
          src="../assets/images/Abou-us-Video.png"
          alt="Leading Companies"
          class="min-w-full h-auto lead-img"
        />
      </div>
    </div>
  </div>
</template>
<script>
import LineReuseable from './LineReuseable.vue'

export default {
  name: 'LeadingSection',
  components: {
    LineReuseable
  }
}
</script>
<style scoped>
@import '../styles/leading.css';
</style>
