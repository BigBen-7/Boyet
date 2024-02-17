<template>
  <section class="case-study-section">
    <div class="container mx-auto">
      <!-- Section Heading -->

      <!-- Case Study Cards -->
      <div class="case-study-container">
        <!-- Loop through case studies and render each card -->
        <div v-for="(caseStudy, index) in caseStudies" :key="index" class="case-study-card">
          <div class="flex">
            <!-- Image -->
            <img :src="caseStudy.image" :alt="caseStudy.title" class="case-img" />
            <!-- Text Container -->
            <div class="text-container" :style="{ backgroundColor: caseStudy.color }">
              <div class="text-content my-10">
                <h3>{{ caseStudy.title }}</h3>
              </div>
              <p>{{ caseStudy.description }}</p>
              <button class="case-btn">Read More</button>
            </div>
          </div>
        </div>
        <button class="read-more-case">Read More Case Studies</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'CaseStudy',
  data() {
    return {
      caseStudies: [
        {
          title: 'Website Design for Shieldedbit Nigeria',
          description:
            'Born out of a vision, a single-minded objective that puts service before anything else, Shieldedbit Nigeria surges forth to deliver the best services in the cyber security and education scenario. Its meteoric rise stems out of a solid foundation. The management boasts of over 20 years of rich and varied experience in the cyber security industry.',
          image: '/src/assets/images/Case-study__web.png',
          color: '#F1F2FF'
        },
        {
          title: 'Website Design for Shieldedbit Nigeria',
          description:
            'Born out of a vision, a single-minded objective that puts service before anything else, Shieldedbit Nigeria surges forth to deliver the best services in the cyber security and education scenario. Its meteoric rise stems out of a solid foundation. The management boasts of over 20 years of rich and varied experience in the cyber security industry.',
          image: '/src/assets/images/Case-study__mobile.png',
          color: '#E7DAED'
        },
        {
          title: 'Website Design for Shieldedbit Nigeria',
          description:
            'Born out of a vision, a single-minded objective that puts service before anything else, Shieldedbit Nigeria surges forth to deliver the best services in the cyber security and education scenario. Its meteoric rise stems out of a solid foundation. The management boasts of over 20 years of rich and varied experience in the cyber security industry.',
          image: '/src/assets/images/Case-study__website.png',
          color: '#FFF4F4'
        }
      ]
    }
  }
}
</script>

<style scoped>
@import '../styles/casestudy.css';
</style>
