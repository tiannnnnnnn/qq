<template>
  <div class="home">

    <el-button @click="goInt" class="button1"> 介紹-> </el-button>
    <el-button @click="goAbout" class="button2"> 查看更多-> </el-button>
    <el-button @click="go3" class="button3"> 查看更多-> </el-button>
    <el-button @click="go4" class="button4"> 查看更多-> </el-button>
    <el-button @click="go5" class="button5"> 馬上預約-> </el-button>
        
    <p1>蘿蔔坑</p1>
    <p2>生態農場</p2>
    <p3>動物</p3>
    <p4>植物</p4>
    <p5>景觀</p5>
    <p66>地址：南投縣埔里鎮種瓜路11之10   /   聯絡電話:049-8765432 </p66>


    <div class = bg><img :src="bgImg1" height=1050px width=1450px></div>
 
    <div class = frog><img :src="bgImg2" height=1050px width=1450px></div>

    <div class = flower><img :src="bgImg3" height=1050px width=1450px></div>

    <div class = rainbow><img :src="bgImg4" height=1050px width=1450px></div>
  </div>
</template>

<script>

export default {

   name: 'App',
   data() {
      return {
         bgImg1: require("../assets/bg.jpg"),
         bgImg2: require("../assets/frog.jpg"),
         bgImg3: require("../assets/flower.jpg"),
         bgImg4: require("../assets/rainbow.jpg"),
      }
   },
    name: "App",
    methods: {
       goInt() {
       this.$router.push("/int");
    },
       goAbout() {
       this.$router.push("/about");
    },
       go3() {
       this.$router.push("/3");
    },
       go4() {
       this.$router.push("/4");
    },
       go5() {
       this.$router.push("/5");
    },
  }
   
}

</script>

<style>

  .button1 {
    position: absolute;
    z-index: 1;
    top: 550px;
    left: 930px;

  }
  .button2 {
    position: absolute;
    z-index: 1;
    top: 1330px;
    left: 430px;

  }
  .button3 {
    position: absolute;
    z-index: 1;
    top: 2320px;
    left: 800px;
  }
  .button4 {
    position: absolute;
    z-index: 1;
    top: 3320px;
     left: 1200px;
  }
  .button5 {
    position: absolute;
    z-index: 1;
    top: 4120px;
    left: 680px;
  }

  .bg img{
    position: absolute;
    top: -100px;
    left: 0px;
  }
  .frog img{
    position: absolute;
    top: 950px;
    left: 0px;
  }
  .flower img{
    position: absolute;
    top: 2000px;
    left: 0px;
  }
  .rainbow img{
    position: absolute;
    top: 3050px;
    left: 0px;
  }

  
  p1{
  position: absolute;
   top: 250px;
   left: 520px;
  font-size: 150px;
  letter-spacing:45px;
  color: white;
   white-space:nowrap;
   font-family:"DFKai-sb";
    z-index: 1;
  }
  p2{
    position: absolute;
    top: 450px;
    left: 685px;
    font-size: 65px;
    letter-spacing:40px;
    color: white;
    white-space:nowrap;
        font-family:"DFKai-sb";
        z-index: 1;
  }
  p3{
    position: absolute;
    top: 1130px;
    left: 280px;
    font-size: 130px;
    letter-spacing:20px;
    color: white;
    font-family:"DFKai-sb";
    white-space:nowrap;
    z-index: 2;
  }
  p4{
    position: absolute;
    top: 2130px;
    left: 657px;
    font-size: 130px;
    letter-spacing:20px;
    color: white;
    font-family:"DFKai-sb";
    white-space:nowrap;
    z-index: 2;
  }
  p5{
    position: absolute;
    top: 3130px;
    left: 1008px;
    font-size: 130px;
    letter-spacing:20px;
    color: white;
    font-family:"DFKai-sb";
    white-space:nowrap;
    z-index: 2;
  }
  p66{
    position: absolute;
    top: 4170px;
    left: 420px;
    font-size: 15px;
    letter-spacing:10px;
    color: rgb(0, 0, 0);
    font-family:"DFKai-sb";
    white-space:nowrap;
    z-index: 2;
  }
 .home{
     margin:0 auto;
  }
</style>
