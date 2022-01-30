<template>
    <div class="background"></div>

    <div class="landingpage">    
        <div class="container-fluid" >
          <div class="row">

<!-- LANDING HEADINGS -->

           <div class="col-sm-auto col-md-auto col-lg- col-xl- col-xxl" id="landingsection" style="padding-top: 18%; text-align: center; ">
               <h1 style="font-size: 68px; color: #FCA311; font-weight: bold;" class="chadheading"><strong>Chad Liam Hendricks</strong></h1><br>
               <h2 style="font-size: 30px; color: #E5E5E5"><strong>Aspiring Full-Stack Developer</strong></h2><br>


               <a href="https://www.linkedin.com/in/chad-hendricks-a7984921b/" target="_blank"><i class="bi bi-linkedin" style="font-size: 40px; color: #FFFFFF; border: none;"></i></a>
               <a href="https://github.com/chadlhendricks" target="_blank"><i class="bi bi-github" style="font-size: 40px; color: #FFFFFF; border: none; margin-left: 10px;"></i></a>
           </div>

<!-- LANDING PAGE PICTURE -->
           <div class="col-sm-auto col-md-auto col-lg- col-xl- col-xxl">
                 <img src="../assets/images/landing_images/thurs1.png" style="height: 100vh; width: 100%; object-fit: cover;" id="thursimg" alt="">
           </div>
          </div>

        </div>        
    </div>
</template>

<script>
export default {
    
}
</script>

<style>

.landingpage {
    background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.322), rgb(20, 0, 0)),
    url(../assets/images/landing_images/backgroundimage-1.png);
    background-size: cover;
    background-attachment:fixed;
    width: 100%;
    margin-left: 240px;
}

.row{
    backdrop-filter: blur(7px);
    }

    
</style>