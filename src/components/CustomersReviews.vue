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
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-8">
      <!-- Loop through customers and display their information -->
      <div v-for="(customer, index) in customers" :key="index" class="text-center">
        <!-- Customer Image -->
        <img :src="customer.image" alt="Customer" class="rounded-full w-32 h-32 mx-auto mb-2" />

        <!-- Five Star Rating -->
        <div class="flex justify-center mb-2"></div>
      </div>
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
          name: 'John Doe',
          image: '/path/to/your/image1.jpg',
          role: 'Web Developer'
        },
        {
          name: 'Jane Smith',
          image: '/path/to/your/image2.jpg',
          role: 'UI/UX Designer'
        },
        {
          name: 'Alex Johnson',
          image: '/path/to/your/image3.jpg',
          role: 'Project Manager'
        },
        {
          name: 'Emily Brown',
          image: '/path/to/your/image4.jpg',
          role: 'Software Engineer'
        },
        {
          name: 'Michael Davis',
          image: '/path/to/your/image5.jpg',
          role: 'QA Tester'
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
@import '../styles/leading.css';
</style>
