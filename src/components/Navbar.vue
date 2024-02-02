<template>
  <header class="text-black mt-10 py-4">
    <div class="container mx-auto flex items-center justify-between">
      <!-- logo -->
      <div>
        <img src="/src/assets/images/Boyet_logo.png" alt="Boyet_Logo" />
      </div>
      <!-- nav-links -->
      <nav class="space-x-4">
        <router-link to="/" class="hover:underline">Our Services</router-link>
        <router-link to="/about" class="hover:underline">Case Studies</router-link>
        <router-link to="/services" class="hover:underline">Hire Us</router-link>
        <!-- contact-us-button  -->
        <button class="bg-blue-950 text-white font-bold px-4 py-4 rounded-md hover: bg-100">
          Contact Us
        </button>
      </nav>
    </div>
  </header>
</template>
<script>
export default {
  name: 'Navbar-links'
}
</script>
<style scoped>
@import '../styles/Nav.css';
</style>
