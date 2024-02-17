<template>
  <section class="customer-review-section my-32">
    <div class="container mx-auto">
      <!-- Section Heading -->
      <div class="customers-heading">
        <LineReuseable class="line" />
        <h2 class="text-3xl mb-4 text-center">
          Why Customers <br />
          <span class="love"> Love Working With Us </span>
        </h2>
      </div>
      <!-- Paragraph -->
      <p class="mb-8 customers-content">
        Without any doubt I recommend Boyet Technologies as one of the best web and mobile solution
        design agencies. One of the best agencies I’ve come across so far. Wouldn’t hesitate to
        introduce their work to someone else.
      </p>
    </div>
    <!-- //////////////////////////////////////////////////////////////////////////////////////////////////////// -->
    <!-- Customer Cards -->
    <div class="flex justify-center gap-8">
      <!-- Loop through customers and display their information -->
      <div v-for="(customer, index) in customers" :key="index" class="text-center customers">
        <!-- Customer Image -->
        <img
          :src="customer.image"
          :alt="customer.name"
          class="rounded-full w-32 h-32 mx-auto mb-2"
        />
        <!-- Rating  -->
        <img :src="customer.rating" :alt="customer.name" class="w-30 mb-2" />

        <!-- Conditional rendering for middle customer -->
        <div v-if="index === Math.floor(customers.length / 2)">
          <h3 class="middle-customer">{{ customer.name }}</h3>
          <p class="middle-role">{{ customer.role }}</p>
        </div>
        <!-- Conditional rendering for other customers -->
        <div v-else>
          <h3 class="other-customer">{{ customer.name }}</h3>
          <p class="role">{{ customer.role }}</p>
        </div>
      </div>
    </div>
    <div class="deco-arrow mx-5">
      <div class="deco-container flex items-center justify-between">
        <img src="/src/assets/logos/Deco-img-arrow.png" alt="arrow" class="left-arrow" />
        <img src="/src/assets/logos/Deco-img-arrow (1).png" alt="arrow" class="right-arrow" />
      </div>
      <h2 class="text-3xl mb-8 text-center case-study-head">
        Our Recent <br />
        <span class="light">Case Studies</span>
      </h2>
    </div>

    <!-- ///////////////////////////////////////////////////////////////////////////////////////////////////////////// -->
  </section>
</template>

<script>
import LineReuseable from './LineReuseable.vue'
export default {
  name: 'CustomersReviews',
  data() {
    return {
      customers: [
        {
          name: 'Michael Musa',
          image: '/src/assets/customers-img/michael.png',
          role: 'Web Developer',
          rating: '/src/assets/customers-img/stars.png'
        },
        {
          name: 'John Smith',
          image: '/src/assets/customers-img/john.png',
          role: 'UI/UX Designer',
          rating: '/src/assets/customers-img/stars.png'
        },
        {
          name: 'Prosper Nwafor',
          image: '/src/assets/customers-img/prosper.png',
          role: 'Software Engineer',
          rating: '/src/assets/customers-img/stars.png'
        },
        {
          name: 'Emily Brown',
          image: '/src/assets/customers-img/grace.png',
          role: 'Software Engineer',
          rating: '/src/assets/customers-img/stars.png'
        },
        {
          name: 'Michael Davis',
          image: '/src/assets/customers-img/tope.png',
          role: 'QA Tester',
          rating: '/src/assets/customers-img/stars.png'
        }
      ]
    }
  },
  components: {
    LineReuseable
  }
}
</script>

<style scoped>
@import '../styles/customer.css';
</style>
