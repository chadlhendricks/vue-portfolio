<template>
  <section>
    <div class="sections">
      <h1 class="headings">Resume</h1>
      <br />

      <!-- Begin: Resume -->
      <div class="container py-5">
        <div class="row">
          <div class="col-md-12">
            <div id="content">
              <ul class="timeline-1 text-black">
                <li class="event" v-for="(resume, index) in resumes" :key="index">
                  <h4 class="mb-3">{{ resume.year }}</h4>
                  <p>{{ resume.institution }}<br /></p>
                  <p>{{ resume.role }}</p>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <!-- End: Resume -->

      <!-- SKILLS CHART -->

      <div class="row" style="width: 80%; margin: auto; font-size: 20px">
        <div
          class="col-sm-auto col-md-auto col-lg- col-xl- col-xxl"
          style="text-align: start; font-size: 20px"
        >
          <h2 style="text-align: start">Soft Skills:</h2>
          <br />

          <i class="bi bi-chevron-right" style="color: rgb(255, 204, 0)"></i
          >Customer Service experience (75%)<br />
          <div class="progress">
            <div
              class="progress-bar bg-warning progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 75%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
          <i class="bi bi-chevron-right" style="color: rgb(255, 204, 0)"></i
          >Problem-solving (80%)<br />
          <div class="progress">
            <div
              class="progress-bar bg-warning progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 80%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
          <i class="bi bi-chevron-right" style="color: rgb(255, 204, 0)"></i
          >Teamwork (90%)<br />
          <div class="progress">
            <div
              class="progress-bar bg-warning progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 90%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
          <i class="bi bi-chevron-right" style="color: rgb(255, 204, 0)"></i
          >Attention to detail (85%)<br />
          <div class="progress">
            <div
              class="progress-bar bg-warning progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 85%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
          <i class="bi bi-chevron-right" style="color: rgb(255, 204, 0)"></i
          >Passion for technology (98%) <br />
          <div class="progress">
            <div
              class="progress-bar bg-warning progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 98%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
          <i class="bi bi-chevron-right" style="color: rgb(255, 204, 0)"></i
          >Adaptable (90%) <br />
          <div class="progress">
            <div
              class="progress-bar bg-warning progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 90%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </div>

        <div
          class="col-sm-auto col-md-auto col-lg- col-xl- col-xxl"
          style="text-align: start; font-size: 20px"
        >
          <h2 style="text-align: start">Technical Skills:</h2>
          <br />

          <i class="bi bi-chevron-right" style="color: red"></i>HTML (80%)<br />
          <div class="progress">
            <div
              class="progress-bar bg-danger progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 80%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
          <i class="bi bi-chevron-right" style="color: red"></i>CSS (70%)<br />
          <div class="progress">
            <div
              class="progress-bar bg-danger progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 70%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
          <i class="bi bi-chevron-right" style="color: red"></i>Javascript
          (60%)<br />
          <div class="progress">
            <div
              class="progress-bar bg-danger progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 60%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
          <i class="bi bi-chevron-right" style="color: red"></i>MySQL (60%)<br />
          <div class="progress">
            <div
              class="progress-bar bg-danger progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 90%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
          <i class="bi bi-chevron-right" style="color: red"></i>Adobe Photoshop
          (70%) <br />
          <div class="progress">
            <div
              class="progress-bar bg-danger progress-bar-striped progress-bar-animated"
              role="progressbar"
              style="width: 90%"
              aria-valuenow="100"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
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
      resumes: null,
    };
  },
  mounted() {
    fetch("https://thurs-app.herokuapp.com/resumes")
      .then((response) => {
        return response.json();
      })
      .then((data) => {
        console.log(data);

        this.resumes = data;
      });
  },
};
</script>

<style scoped>
/* 
Color Palette
#000000 - Black
#14213D - Blue
#FCA311 - Orange
#E5E5E5 - Grey
#FFFFFF - White
*/
.row {
  color: white;
}

h2 {
  color: #fca311ff;
}

h4 {
  color: #fca311ff;
}

.timeline-1 {
  border-left: 3px solid #fca311ff;
  border-bottom-right-radius: 4px;
  border-top-right-radius: 4px;
  background: rgba(177, 99, 163, 0.048);
  margin: 0 auto;
  position: relative;
  padding: 50px;
  list-style: none;
  text-align: left;
  max-width: 40%;
}

@media (max-width: 767px) {
  .timeline-1 {
    max-width: 98%;
    padding: 25px;
  }
}

.timeline-1 .event {
  border-bottom: 1px dashed #000;
  padding-bottom: 25px;
  margin-bottom: 25px;
  position: relative;
}

@media (max-width: 767px) {
  .timeline-1 .event {
    padding-top: 30px;
  }
}

.timeline-1 .event:last-of-type {
  padding-bottom: 0;
  margin-bottom: 0;
  border: none;
}

.timeline-1 .event:before,
.timeline-1 .event:after {
  position: absolute;
  display: block;
  top: 0;
}

.timeline-1 .event:before {
  left: -207px;
  content: attr(data-date);
  text-align: right;
  font-weight: 100;
  font-size: 0.9em;
  min-width: 120px;
}

@media (max-width: 767px) {
  .timeline-1 .event:before {
    left: 0px;
    text-align: left;
  }
}

.timeline-1 .event:after {
  -webkit-box-shadow: 0 0 0 3px #b565a7;
  box-shadow: 0 0 0 3px #b565a7;
  left: -55.8px;
  background: #fff;
  border-radius: 50%;
  height: 9px;
  width: 9px;
  content: "";
  top: 5px;
}

@media (max-width: 767px) {
  .timeline-1 .event:after {
    left: -31.8px;
  }
}
</style>
