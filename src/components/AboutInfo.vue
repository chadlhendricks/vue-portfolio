<template>
  <section>
    <div class="sections">
      <h1 class="headings">About</h1>
      <br />

      <div class="container-fluid">
        <div class="row" id="landingpagerows" style="padding-top: 20px">
          <!-- ABOUT PAGE PICTURE -->

          <div class="col-md-6 col-sm-12" id="imgdiv">
            <img
              src="../assets/images/about_images/chad.png"
              id="aboutpic"
              style=""
              alt=""
            />
          </div>

          <!-- ABOUT PAGE PARAGRAPHS -->

          <div
            class="col-md-6 col-sm-12"
            id="aboutparag"
          >
            <p
              style="
                color: crimson;
                text-align: start;
                font-size: 20px;
                font-weight: bold;
              "
            >
              Bio
            </p>
            <p style="text-align: start; font-size: 20px">
              I am a hard-working, inquisitive and creative-thinking individual.
              I always try to stimulate my brain, learn new things and be
              productive. Furthermore, I enjoy helping others and working
              together to solve issues. I&#39;m introverted, but I try to push
              myself out of my comfort zone so that I can experience new people
              and things.
            </p>
            <br />

            <p
              style="
                color: crimson;
                text-align: start;
                font-size: 20px;
                font-weight: bold;
              "
            >
              Where did your passion for coding start:
            </p>
            <p style="text-align: start; font-size: 20px">
              My passion for the tech industry came from video games. I was
              always curious when I went into game directory files and saw
              things like sprites, models and background images and wondered how
              it was pieced together to make the games I enjoyed. Eventually, I
              started watching videos on YouTube, people showing how they would
              make games and websites from scratch and I figured that it was
              something I&#39;d enjoy doing.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>

#imgdiv{
  margin: auto;
}
#aboutpic {
  text-align: center;
  border-radius: 50%;
  height: 60vh;
  border: 10px crimson double;
  -webkit-animation: scale-up-center 0.4s cubic-bezier(0.39, 0.575, 0.565, 1)
    both;
  animation: scale-up-center 0.4s cubic-bezier(0.39, 0.575, 0.565, 1) both;
}

@media (min-width: 1400px) {
  .sections {
    margin-left: 0;
  }
  #aboutpic {
    margin-left: 200px;
  }
}

@-webkit-keyframes scale-up-center {
  0% {
    -webkit-transform: scale(0.5);
    transform: scale(0.5);
  }
  100% {
    -webkit-transform: scale(1);
    transform: scale(1);
  }
}
@keyframes scale-up-center {
  0% {
    -webkit-transform: scale(0.5);
    transform: scale(0.5);
  }
  100% {
    -webkit-transform: scale(1);
    transform: scale(1);
  }
}
</style>
