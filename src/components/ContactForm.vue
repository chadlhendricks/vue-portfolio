<template>
<section>
    <h1 class="headings">Contact Me</h1><br>

   <div class="contactform col-sm-6" style="font-size: 20px;">
        <form action="https://formspree.io/f/xzbywdvz" method="POST">
          
          <div class="row">
            <div class="mb-3 col-6">
              <label for="fullname" class="form-label">Full Name:</label>
              <input type="text" class="form-control" id="fullname" name="fullname" aria-describedby="emailHelp" required="">
            </div>

            <div class="mb-3 col-6">
              <label for="exampleInputEmail1" class="form-label">Email address:</label>
              <input type="email" class="form-control" id="exampleInputEmail1" name="emailaddress" aria-describedby="emailHelp" required="">
            </div>
          </div>

          <div class="mb-3">
              <label for="messagebox" class="form-label">Message:</label>
              <input type="textarea" class="form-control" id="messagebox" name="message" required="">
          </div>

          <div class="mb-3 form-check" style="text-align:center">
            <button type="submit" class="btn btn-danger">Submit</button>
          </div>
  
        </form>

      </div>
      </section>


</template>


<script>
export default {
    data(){
        return {
            email: '',
            role: '',
            terms: false,
            tempSkill: '',
            skills: []            
        }
    },
        methods: {
        addSkill(e) {
            if(e.key === "," && this.tempSkill) {
                this.skills.push(this.tempSkill);
                this.tempSkill = "";
            }
        }
    }
    
}
</script>
<style>
.contactform.col-sm-6 {
    padding-top: 100px;
    margin: auto;
    width: 80%;
}
   
</style>