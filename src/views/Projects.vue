<template>
  <div class="projects">
    <Navbar/>
    <ProjectsList/>

  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import ProjectsList from '@/components/ProjectsList.vue'



export default {
  name: 'Projects',
  components: {
    Navbar, ProjectsList
  }
}
</script>