<template>
<section>
    <div class="sections">
        <h1 class="headings">Resume</h1><br>

        <div class="container py-5">
  <div class="row">
    <div class="col-md-12">
      <div id="content">
        <ul class="timeline-1 text-black">
          <li class="event" data-date="12:30 - 1:00pm">
            <h4 class="mb-3">Registration</h4>
            <p>Get here on time, it's first come first serve. Be late, get turned away.</p>
          </li>
          <li class="event" data-date="2:30 - 4:00pm">
            <h4 class="mb-3 pt-3">Opening Ceremony</h4>
            <p>Get ready for an exciting event, this will kick off in amazing fashion with MOP &amp; Busta
              Rhymes as an opening show.</p>
          </li>
          <li class="event" data-date="5:00 - 8:00pm">
            <h4 class="mb-3 pt-3">Main Event</h4>
            <p>This is where it all goes down. You will compete head to head with your friends and rivals. Get
              ready!</p>
          </li>
          <li class="event" data-date="8:30 - 9:30pm">
            <h4 class="mb-3 pt-3">Closing Ceremony</h4>
            <p class="mb-0">See how is the victor and who are the losers. The big stage is where the winners bask in their
              own glory.</p>
          </li>
        </ul>
      </div>
    </div>
  </div>
</div>

<!-- SKILLS CHART -->

<div class="row" style="width: 80%; margin: auto; font-size: 20px;">

        <div class="col-sm-auto col-md-auto col-lg- col-xl- col-xxl" style="text-align: start; font-size: 20px;">
          <h2 style="text-align: start;">Soft Skills:</h2><br>

          <i class="bi bi-chevron-right" style="color: rgb(255,204,0);"></i>Customer Service experience (75%)<br>
            <div class="progress">
              <div class="progress-bar bg-warning progress-bar-striped progress-bar-animated" role="progressbar" style="width: 75%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <i class="bi bi-chevron-right" style="color: rgb(255,204,0);"></i>Problem-solving (80%)<br>
            <div class="progress">
              <div class="progress-bar bg-warning progress-bar-striped progress-bar-animated" role="progressbar" style="width: 80%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <i class="bi bi-chevron-right" style="color: rgb(255,204,0);"></i>Teamwork (90%)<br>
            <div class="progress">
              <div class="progress-bar bg-warning progress-bar-striped progress-bar-animated" role="progressbar" style="width: 90%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <i class="bi bi-chevron-right" style="color: rgb(255,204,0);"></i>Attention to detail (85%)<br>
            <div class="progress">
              <div class="progress-bar bg-warning progress-bar-striped progress-bar-animated" role="progressbar" style="width: 85%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <i class="bi bi-chevron-right" style="color: rgb(255,204,0);"></i>Passion for technology (98%) <br>
            <div class="progress">
              <div class="progress-bar bg-warning progress-bar-striped progress-bar-animated" role="progressbar" style="width: 98%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <i class="bi bi-chevron-right" style="color: rgb(255,204,0);"></i>Adaptable (90%) <br>
            <div class="progress">
              <div class="progress-bar bg-warning progress-bar-striped progress-bar-animated" role="progressbar" style="width: 90%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
        </div>


        <div class="col-sm-auto col-md-auto col-lg- col-xl- col-xxl" style="text-align: start; font-size: 20px;">
          <h2 style="text-align: start;">Technical Skills:</h2><br>

          <i class="bi bi-chevron-right" style="color: red;"></i>HTML (80%)<br>
            <div class="progress">
              <div class="progress-bar bg-danger progress-bar-striped progress-bar-animated" role="progressbar" style="width: 80%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <i class="bi bi-chevron-right" style="color: red;"></i>CSS (70%)<br>
            <div class="progress">
              <div class="progress-bar bg-danger progress-bar-striped progress-bar-animated" role="progressbar" style="width: 70%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <i class="bi bi-chevron-right" style="color: red;"></i>Javascript (40%)<br>
            <div class="progress">
              <div class="progress-bar bg-danger progress-bar-striped progress-bar-animated" role="progressbar" style="width: 40%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <i class="bi bi-chevron-right" style="color: red;"></i>MySQL (60%)<br>
            <div class="progress">
              <div class="progress-bar bg-danger progress-bar-striped progress-bar-animated" role="progressbar" style="width: 90%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
            <i class="bi bi-chevron-right" style="color: red;"></i>Adobe Photoshop (70%) <br>
            <div class="progress">
              <div class="progress-bar bg-danger progress-bar-striped progress-bar-animated" role="progressbar" style="width: 90%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
        </div>
  
      </div>

        

        

    </div>
</section>

</template>

<script>
export default {
    
}
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

.timeline-1 {
  border-left: 3px solid #FCA311;
  border-bottom-right-radius: 4px;
  border-top-right-radius: 4px;
  background: rgba(177, 99, 163, 0.09);
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