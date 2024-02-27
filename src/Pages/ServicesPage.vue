<template>
  <section>
    <div class="Service-page flex items-center justify-center my-10">
      <!-- Text and image container  -->
      <div class="container mx-auto flex flex-col lg:flex-row items-center justify-center">
        <!-- Text Content  -->
        <div class="text-content lg:w-1/2 lg:pr-8">
          <h1 class="text-3xl font-medium mb-4 services-head lite">
            Do <span class="bold">it</span> the <br />
            <span class="black bold">boyet </span>
            <span class="bold">way!</span>
          </h1>
          <p class="text-gray-700 mb-8 head-content">
            Design and develop your web and mobile applications efficiently with an amazing team
            that leaves nothing out of the picture. From designing, to development and final lunch.
          </p>
          <!-- Button with Arrow Icon -->
          <div class="services-btn py-8">
            <div class="btn flex">
              <button class="flex items-center px-10 service-btn">Get started</button>
              <button class="flex items-center px-10 service-btn">Contact us</button>
            </div>
          </div>
        </div>
        <!-- Image -->
        <div class="image-container lg:w-1/2 lg:pl-8">
          <img
            src="../assets/ServicesImages/image 36.png"
            alt="Leading Companies"
            class="min-h-fit h-auto lead-img"
          />
        </div>
      </div>
    </div>
  </section>
  <section>
    <div class="expert-head text-center">
      <LineReuseable class="line" />
      <h2>We are <span class="expert">Experts</span></h2>
    </div>
    <!-- ExPERTISE  -->

    <div class="expertise-section my-20">
      <!-- Text and image container  -->
      <div class="container mx-auto flex flex-col lg:flex-row items-center justify-around">
        <!-- Text Content  -->
        <div class="text-content lg:w-1/2 lg:pr-8">
          <h1 class="text-3xl font-medium expertise-head">Web Design & Development</h1>
          <p class="expertise-para">
            A Website is an extension of yourself and we can help you to express it properly. Your
            website is your number one marketing asset because we live in a digital age. A Website
            is an extension of yourself and we can help you to express it properly. Your website is
            your number one marketing asset because we live in a digital age.
          </p>
        </div>
        <!-- Image -->
        <div class="image-container relative">
          <!-- <img src="../assets/ServicesImages/image 4 (1).png" alt="" class="image1" /> -->
          <img
            src="../assets/ServicesImages/image 4.png"
            alt="Leading Companies"
            class="expert-img rounded-lg image2"
          />
        </div>
      </div>

      <!-- CARD TWO  -->
      <div class="container mx-auto flex flex-col lg:flex-row items-center justify-around py-10">
        <!-- Image -->
        <div class="image-container">
          <!-- <img src="../assets/ServicesImages/image 4 (1).png" alt="" class="image1" /> -->
          <img
            src="../assets/ServicesImages/image 4 (1).png"
            alt="Leading Companies"
            class="expert-img rounded-lg image2"
          />
        </div>

        <div class="text-content lg:w-1/2 lg:pr-8">
          <h1 class="text-3xl font-medium expertise-head">Mobile App Development</h1>
          <p class="expertise-para">
            A Website is an extension of yourself and we can help you to express it properly. Your
            website is your number one marketing asset because we live in a digital age. A Website
            is an extension of yourself and we can help you to express it properly. Your website is
            your number one marketing asset because we live in a digital age.
          </p>
        </div>
      </div>

      <!-- CARD THREE  -->
      <div class="container mx-auto flex flex-col lg:flex-row items-center justify-around py-10">
        <div class="text-content lg:w-1/2 lg:pr-8">
          <h1 class="text-3xl font-medium expertise-head">Software Testing Services</h1>
          <p class="expertise-para">
            A Website is an extension of yourself and we can help you to express it properly. Your
            website is your number one marketing asset because we live in a digital age. A Website
            is an extension of yourself and we can help you to express it properly. Your website is
            your number one marketing asset because we live in a digital age.
          </p>
        </div>
        <!-- Image -->
        <div class="image-container">
          <!-- <img src="../assets/ServicesImages/image 4 (1).png" alt="" class="image1" /> -->
          <img
            src="../assets/logos/Mask Group.png"
            alt="Leading Companies"
            class="expert-img rounded-lg image2"
          />
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import LineReuseable from '@/components/LineReuseable.vue'

export default {
  name: 'ServicesPage',
  components: {
    LineReuseable
  }
}
</script>
<style scoped>
@import '../pagesStyles/Services.css';
</style>
