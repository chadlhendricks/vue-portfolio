<template>
    <Navbar/>
    <ListProjects/>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import ListProjects from '@/components/ListProjects.vue'



export default {
  name: 'Projects',
  components: {
    Navbar, ListProjects
  }
}
</script>