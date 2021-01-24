<template>
  <div class="about">
    <el-button @click="goHome" class="button10"> Home </el-button>
     <div class = allAnimals><img :src="bgImg1" height=1250px width=1450px></div>
      <div class = square2></div>
       <h11> 蘿蔔坑有各式各樣的野生動物，</h11>
       <h12> 他們自願前來，把這當作自己的家。</h12>
  </div>
</template>

<script>

export default {

    name: "App",
    data() {
      return {
         bgImg1: require("../assets/allAnimals.jpg"),
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
  .square2 {
      height: 220px;
      width: 720px;
      border-radius: 20px;
      position: absolute;
      top: 200px;
      left: 310px;
      background-color: rgb(255, 255, 255);
      z-index: 2;
      opacity: 0.5;
  }
  .button10 {
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
   h11{
    z-index: 8;
    position: absolute;
    left: 360px;
    top: 250px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 10px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
   h12{
    z-index: 8;
    position: absolute;
    left: 360px;
    top: 320px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 10px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
   .about{
     margin:0 auto;
  }
</style>
