<template>
  <div class="about">
    <el-button @click="goHome" class="button7"> Home </el-button>
     <div class = allAnimals><img :src="bgImg1" height=1050px width=1450px></div>
  <div class = square3></div>
   <h21> 這裡的植物多為自然生長，</h21>
   <h22> 即便是人工種植也堅持使用天然方法。</h22>
  </div>
  
</template>

<script>

export default {

    name: "App",
    data() {
      return {
         bgImg1: require("../assets/allFlowers.jpg"),
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
 h21{
    z-index: 8;
    position: absolute;
    left: 360px;
    top: 420px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 10px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
  h22{
    z-index: 8;
    position: absolute;
    left: 360px;
    top: 490px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 7px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
  .square3 {
      height: 210px;
      width: 720px;
      border-radius: 20px;
      position: absolute;
      top: 380px;
      left: 310px;
      background-color: rgb(255, 255, 255);
      z-index: 2;
      opacity: 0.5;
  }
  .button7 {
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
   .about{
     margin:0 auto;
  }
</style>
