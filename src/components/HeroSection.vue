<template>
  <section class="hero-section flex items-center justify-evenly mt-9 p-4">
    <!-- Hero-left-side Text-content  -->
    <div class="hero-wrapper-text">
      <h1 class="hero-head text-3xl mb-4">
        Great <span class="gradient-text">Product</span> are <br />
        <span class="black-bold-text"> built by great </span>
        <span class="gradient-text">teams</span>
      </h1>
      <p class="hero-detail text-gray-600 mb-8">
        We help build and manage a team of world class developers <br />
        to bring your vision to life.
      </p>
      <button class="px-6 py-3 rounded-md hero-btn">Let's Get Started</button>
    </div>
    <!-- Hero-Right-Side: Stacked-images   -->
    <div class="image-container">
      <img src="../assets/images/coding woman-bg.png" alt="Woman Coding" class="mb-4" />
      <img src="../assets/images/Group 451.png" alt="" class="group-image" />
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroSection'
}
</script>

<style scoped>
@import '../styles/Hero.css';
</style>
