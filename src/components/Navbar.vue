<template>
<div class="s-layout">
<!-- Sidebar -->
<div class="s-layout__sidebar">
  <a class="s-sidebar__trigger" href="#0">
     <i class="fa fa-bars"></i>
  </a>

  <nav class="s-sidebar__nav">
     <ul>
        <li>
           <router-link to="/" class="s-sidebar__nav-link">
             <i class="bi bi-house-fill"></i><em>Home</em>
           </router-link>
        </li>
        <li>
           <router-link to="/about" class="s-sidebar__nav-link">
             <i class="fa fa-user"></i><em>About</em>
           </router-link>
        </li>
        <li>
           <router-link to="/resume" class="s-sidebar__nav-link">
              <i class="bi bi-pencil-square"></i><em>Resume</em>
           </router-link>
        </li>
         <li>
           <router-link to="/projects" class="s-sidebar__nav-link">
              <i class="bi bi-file-earmark-code-fill"></i><em>Projects</em>
           </router-link>
        </li>
         <li>
           <router-link to="/testimonials" class="s-sidebar__nav-link">
              <i class="bi bi-people-fill"></i><em>Testimonials</em>
           </router-link>
        </li>
         <li>
           <router-link to="/contact" class="s-sidebar__nav-link">
              <i class="bi bi-chat"></i><em>Contact</em>
           </router-link>
        </li>
     </ul>
  </nav>
</div>
</div>
      
</template>

<script>

</script>

<style scoped>


*, *::before, *::after {
   box-sizing: border-box;
}

.bi, .fa {
  color: #FCA311
  }

body {
   font-size: 1em;
   color: #333;
}

em {
   font-style: normal;
}

a {
   text-decoration: none;
   color: inherit;
} 

/* Layout */
.s-layout {
   display: flex;
   width: 100%;
}

.s-layout__content {
   display: flex;
   justify-content: center;
   align-items: center;
   flex: 1;
}

/* Sidebar Closing*/
.s-sidebar__trigger {
   z-index: 2;
   position: fixed;
   top: 0;
   left: 0;
   width: 100%;
   height: 4em;
   background: #000000;
}

/* Burger Menu */
.s-sidebar__trigger > i {
   display: inline-block;
   margin: 1.5em 0 0 1.5em;
   color: #FCA311;
}

/* Sidebar Expanded Color */
.s-sidebar__nav {
   position: fixed;
   top: 0;
   left: -15em;
   overflow: hidden;
   transition: all .3s ease-in;
   width: 15em;
   height: 100%;
   background: #000000;
   color: rgba(255, 255, 255, 0.7);
}

.s-sidebar__nav:hover,
.s-sidebar__nav:focus,
.s-sidebar__trigger:focus + .s-sidebar__nav,
.s-sidebar__trigger:hover + .s-sidebar__nav {
   left: 0;
}

.s-sidebar__nav ul {
   position: absolute;
   top: 4em;
   left: 0;
   margin: 0;
   padding: 0;
   width: 15em;
}

.s-sidebar__nav ul li {
   width: 100%;
}

.s-sidebar__nav-link {
   position: relative;
   display: inline-block;
   width: 100%;
   height: 4em;
}

.s-sidebar__nav-link em {
   position: absolute;
   top: 50%;
   left: 4em;
   transform: translateY(-50%);
}

/* Sidemenu Hover */

.s-sidebar__nav-link:hover {
   background: #FCA311;
}

.s-sidebar__nav-link > i {
   position: absolute;
   top: 0;
   left: 0;
   display: inline-block;
   width: 4em;
   height: 4em;
}

.s-sidebar__nav-link > i::before {
   position: absolute;
   top: 50%;
   left: 50%;
   transform: translate(-50%, -50%);
}

/* Mobile First */
@media (min-width: 42em) {
   .s-layout__content {
      margin-left: 4em;
   }
   
   /* Sidebar */
   .s-sidebar__trigger {
      width: 4em;
   }
   
   .s-sidebar__nav {
      width: 4em;
      left: 0;
   }
   
   .s-sidebar__nav:hover,
   .s-sidebar__nav:focus,
   .s-sidebar__trigger:hover + .s-sidebar__nav,
   .s-sidebar__trigger:focus + .s-sidebar__nav {
      width: 15em;
   }
}

@media (min-width: 68em) {
   .s-layout__content {
      margin-left: 15em;
   }
   
   /* Sidebar */
   .s-sidebar__trigger {
      display: none
   }
   
   .s-sidebar__nav {
      width: 15em;
   }
   
   .s-sidebar__nav ul {
      top: 1.3em;
   }
}




</style>
