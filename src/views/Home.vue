<template>
<Navbar/>
<LandingPage/>


</template>

<script>
import Navbar from '@/components/Navbar.vue'
import LandingPage from '@/components/LandingPage.vue'



export default {
  name: 'Home',
  components: {
    Navbar, LandingPage
  }
}
</script>

<style scoped>



#landingimage {
  height: 90vh;
  overflow-y: hidden;
  width: 100%;
  top: 0;
  /* filter: brightness(0.4); */
  top: 0;


  object-fit: cover;
}


</style>
