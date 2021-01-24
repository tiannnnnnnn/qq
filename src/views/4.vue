<template>
  <div class="about">
    <el-button @click="goHome" class="button8"> Home </el-button>
     <div class = allAnimals><img :src="bgImg1" height=1250px width=1450px></div>
      <h31>在這裡，無論是俯瞰市景、遠眺山景、</h31>
      <h32> 甚至是觀賞日落，你都能一次享受。</h32>
       <div class = square4></div>
  </div>
</template>

<script>

export default {

    name: "App",
    data() {
      return {
         bgImg1: require("../assets/allSight.jpg"),
      }
   },
    methods: {
       goHome() {
       this.$router.push("/");
    },
  }
   
}
</script>

<style>
h31{
    z-index: 8;
    position: absolute;
    left: 350px;
    top: 420px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 10px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
  h32{
    z-index: 8;
    position: absolute;
    left: 350px;
    top: 480px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 4.8px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
  .button8 {
        position: absolute;
        z-index: 5;
        top: 40px;
        left: 30px;
  }
  .allAnimals img{
    position: absolute;
    top: -100px;
    left: 0px;
  }
  .square4 {
      height: 210px;
      width: 750px;
      border-radius: 20px;
      position: absolute;
      top: 380px;
      left: 310px;
      background-color: rgb(255, 255, 255);
      z-index: 2;
      opacity: 0.5;
  }
   .about{
     margin:0 auto;
  }
</style>
