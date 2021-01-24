<template>
  <div class="about">
    <h6>「蘿蔔坑」是從南投縣埔里鎮山上一塊蘿蔔田蛻變成的生態農場。</h6>
    <h2> 這塊堅持不用化肥、農藥、殺蟲劑的土地，是許多昆蟲、動物的棲息地。</h2>
    <h3> 無論早晚、無論何種季節，這裡永遠有絕佳的景色。</h3>
    <h4> 想體會和自然和平共處的感覺、帶孩子親眼認識更多的植物、動物，</h4>
    <h5> 或是單純來觀景修養身心，蘿蔔坑都是絕佳的選擇。</h5>
    
    <el-button @click="goHome" class="button6"> Home </el-button>
     <div class = allAnimals><img :src="bgImg1" height=1050px width=1450px></div>
 <div class = square></div>
  </div> 
</template>

<script>

export default {

    name: "App",
    data() {
      return {
         bgImg1: require("../assets/bg.jpg"),
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
  .square {
      height: 950px;
      width: 1450px;
      position: absolute;
      top: 0px;
      left: 0px;
      background-color: rgb(255, 255, 255);
      z-index: 2;
      opacity: 0.7;
  }
  .button6  {
        position: absolute;
        z-index: 3;
        top: 40px;
        left: 30px;
  }
  .allAnimals img{
    z-index: 1;
    position: absolute;
    top: -100px;
    left: 0px;
  }
  h6{
    z-index: 8;
    position: absolute;
    left: 130px;
    top: 150px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 10px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
  h2{
    z-index: 8;
    position: absolute;
    left: 160px;
    top: 280px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 4.8px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
  h3{
    z-index: 8;
    position: absolute;
    left: 160px;
    top: 360px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 19.3px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
  h4{
    z-index: 8;
    position: absolute;
    left: 160px;
    top: 440px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 7.3px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
  h5{
    z-index: 8;
    position: absolute;
    left: 160px;
    top: 520px;
    white-space:nowrap;
    font-size: 30px;
    letter-spacing: 19.3px;
    font-family:"DFKai-sb";
    font-weight:bold;
  }
  .about{
     margin:0 auto;
  }
</style>
