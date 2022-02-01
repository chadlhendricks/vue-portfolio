<template>

<section>
     <div class="sections">
        <h1 class="headings">Testimonials</h1><br>
     </div> 

     <MDBCarousel
    v-model="carousel1"
    :items="items1"
    fade
  />


</section>

</template>

<script>

import { ref } from "vue";
  import { MDBCarousel } from "mdb-vue-ui-kit";
  export default {
    components: {
      MDBCarousel
    },
    setup() {
      const items1 = [
        {
          src: "https://user-images.githubusercontent.com/7884263/27209183-2f456e10-51ff-11e7-9ec3-847038a795ea.png",
          alt: "Sergio Rodgers",
          label: "- Sergio Rodgers",
          caption: "In the short time I’ve know Chad I’ve come to see how good he is at adapting to new things and how good he is at socialising with peers. Chad is an amazing Individual that is committed and he would be an amazing asset to any company.Nulla vitae elit libero, a pharetra augue mollis interdum."
        },
        {
          src: "https://user-images.githubusercontent.com/7884263/27209183-2f456e10-51ff-11e7-9ec3-847038a795ea.png",
          alt: "Daryll Grainger",
          label: "- Daryll Grainger",
          caption: "Chad is great at what he does.Lorem ipsum dolor sit amet, consectetur adipiscing elit."
        },
        {
          src: "https://user-images.githubusercontent.com/7884263/27209183-2f456e10-51ff-11e7-9ec3-847038a795ea.png",
          alt: "Siyanda Ncamazana",
          label: "- Siyanda Ncamazana",
          caption:
            "Chad is an extremely hard worker and is open minded learning new things. He is not afraid of challenges and is willing to go the extra mile.Praesent commodo cursus magna, vel scelerisque nisl consectetur."
        },
        {
          src: "https://user-images.githubusercontent.com/7884263/27209183-2f456e10-51ff-11e7-9ec3-847038a795ea.png",
          alt: "Siyabonga Mkhosana",
          label: "Siyabonga Mkhosana",
          caption:
            "Chad Hendricks has shown a capacity to learn quick and work efficiency, has a good work ethic and ability to work in a team. Very dependable and committed."
        },
        {
          src: "https://user-images.githubusercontent.com/7884263/27209183-2f456e10-51ff-11e7-9ec3-847038a795ea.png",
          alt: "Godwin Dzvapatsva",
          label: "- Godwin Dzvapatsva -Head of Curriculum and Learning",
          caption:
            "Chad has the potential to do well is his studies."
        }
      ];
      const carousel1 = ref(0);
      return {
        items1, carousel1
      };
    }
  };

</script>

<style scoped>


</style>