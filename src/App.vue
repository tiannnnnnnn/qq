<template>
  <div id="app">
     <!-- <div id="nav">
         <router-link to="/">Home</router-link>   |
         <router-link to="/about">About</router-link>   |
         <router-link to="/week10">Week10</router-link>
      </div> -->
        <router-view/>

  </div>
  
</template>

<script>

export default {
  
}

</script>

<style>

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.homee{
  top: 4150px;
}



#nav a {
  z-index: 1;
  font-weight: bold;
  color: #2c3e50;
  
}
#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
