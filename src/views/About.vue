<template>
    <Navbar/>
    <AboutInfo/>
    <Footer/>

</template>

<script>
import Navbar from '@/components/Navbar.vue'
import AboutInfo from '@/components/AboutInfo.vue'
import Footer from '@/components/Footer.vue'


export default {
  name: 'About',
  components: {
    Navbar, AboutInfo, Footer }
}
</script>


<style>


</style>
