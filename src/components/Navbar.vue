<template>

<header>
        <nav class="navbar navbar-expand-lg navbar-light fixed-top" style="background-color: rgba(0, 0, 0, 1);">
            <div class="container-fluid">
              <a class="navbar-brand" href="#landing"><img src="../assets/images/logos/logo-1.png" width="80%"></a>
              <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
              <div class="collapse navbar-collapse" style="justify-content: flex-end; height: 100%;" id="navbarSupportedContent">
                <ul class="navbar-nav mb-2 mb-lg-0">
                  <router-link to="/"><i class="bi bi-house-fill"></i> Home</router-link>
                  <router-link to="/about"><i class="bi bi-person-circle"></i> About</router-link>
                  <router-link to="/resume"><i class="bi bi-file-richtext-fill"></i> Resume</router-link>
                  <router-link to="/projects"><i class="bi bi-person-workspace"></i> Projects</router-link>
                  <router-link to="/testimonials"><i class="bi bi-people-fill"></i> Testimonials</router-link>
                  <router-link to="/contact"><i class="bi bi-chat-dots-fill"></i> Contact</router-link>
                </ul>
              </div>
            </div>
          </nav>         
    </header>

</template>

<script>


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: red;
}
</style>
