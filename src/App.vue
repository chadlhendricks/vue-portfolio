<template>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
}

#nav {
  margin: 0;
}

#nav a {
  font-weight: bold;
  margin-left: 20px;
  color: whitesmoke;
}

#nav a.router-link-exact-active {
  color: red;
  font-size: 20px;
  border: 3px red solid;
  border-top: none;
  border-left: none;
  border-right: none;
  font-style:;
}
.container-fluid{
  background-color: rgba(0, 0, 0, 0.26) ;
}
</style>
