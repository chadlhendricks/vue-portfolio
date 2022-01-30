<template>
<div class="about">
  <Navbar/>
  <TestimonialCarousel/>

</div>

</template>

<script>
import Navbar from '@/components/Navbar.vue'
import TestimonialCarousel from '@/components/TestimonialCarousel.vue'


export default {
  name: 'Testimonials',
  components: {
    Navbar, TestimonialCarousel
  }
}

</script>

<style scoped>

</style>

