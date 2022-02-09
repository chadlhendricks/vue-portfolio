<template>
  <div class="resume">
    <Navbar />
    <MyResume />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import MyResume from "@/components/MyResume.vue";

export default {
  name: "Resume",
  components: {
    Navbar,
    MyResume,
  },
  data() {
    return {};
  },
  mounted() {
    fetch("http://localhost:1234")
      .then((response) => {
        console.log("hey");
        return response.json();
      })
      .then((data) => {
        console.log("hey");
        console.log(data);
      });
  }
};
</script>
