<template>
  <section>
    <div class="sections">
      <h1 class="headings">Projects</h1>
      <br />

      <div
        class="row"
        style="
          text-align: center;
          width: 100%;
          margin: auto;
          color: white;
          padding-top: 20px;
        "
      >
        <div class="col-sm-auto col-md-auto col-lg- col-xl- col-xxl">
          <div
            class="card"
            style="width: 30%; border: none; display: inline-block; margin-right: 50px; margin-bottom: 50px "
            v-for="(project, index) in projects"
            :key="index"
          >
            <img
              class="card-img-top"
              :src="project.img"
              alt="Card image cap"
              style="height: 300px"
            />
            <div class="card-body" style="height: 250px">
              <h5 class="card-title">{{ project.projname }}</h5>
              <p class="card-text">{{ project.projdesc }}</p>
            <div class="card-buttons">
              <a :href="project.github" target="_blank" class="btn btn-danger"
                ><i
                  class="bi bi-github"
                  style="font-size: 30px; color: white; border: none"
                ></i
              ></a>
              <a
                :href="project.netlify"
                target="_blank"
                class="btn btn-danger"
                style="display: inline-block"
                ><img
                  src="../assets/images/logos/netlify.png"
                  style="height: 45px; width: 35px"
             ></a>
            </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: null,
    };
  },
  mounted() {
    fetch("https://thurs-app.herokuapp.com/projects")
      .then((response) => {
        return response.json();
      })
      .then((data) => {
        console.log(data);

        this.projects = data;
      });
  },
};
</script>

<style scoped>

.card-buttons{
  position: absolute;
  right:    0;
  bottom:   0;
}

.card {
  color: #fca311;
}

p {
  color: grey;
}

.card-img-top {
  height: 300px;
}
</style>
