<template>
  <div class="about">
    <h1>點選想預約的日期</h1>
    <el-button type="info" @click="goHome" class="button9"> Home </el-button>
     <el-calendar class="cal" ></el-calendar>
  </div>
</template>

<script>

export default {

    name: "App",
    methods: {
       goHome() {
       this.$router.push("/");
    },
  }
   
}
</script>

<style>
  .button9 {
        position: absolute;
        z-index: 5;
        top: 20px;
        left: 20px;
  }
   .about{
     margin:0 auto;
  }
</style>
