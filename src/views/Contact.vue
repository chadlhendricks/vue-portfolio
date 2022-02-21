<template>
  <Navbar/>
  <ContactForm/>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import ContactForm from '@/components/ContactForm.vue'
import Footer from '@/components/Footer.vue'



export default {
  name: 'Contact',
  components: {
    ContactForm, Navbar, Footer
  }
}
</script>


