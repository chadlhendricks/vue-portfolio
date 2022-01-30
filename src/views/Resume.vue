<template>
  <div class="resume">
    <Navbar/>
    <MyResume/>

  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import MyResume from '@/components/MyResume.vue'



export default {
  name: 'Resume',
  components: {
    Navbar, MyResume
  }
}
</script>
