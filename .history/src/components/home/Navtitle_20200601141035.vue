<template>
 <div class="full-page">
<div class="col">
<div class="logo"><img src="https://static.shiyanlou.com/frontend/dist/img/9f43b00.svg" alt="实验楼" ></div>
<span class="slogan">做实验，学编程</span>
<div style="width:500px;height:100px"></div>
<span class="nav-link-enterprise">企业版</span>
<span class="nav-link"></span>
<span class="nav-link-enterprise">学校版</span>
</div>
 
 </div>
</template>

<script>
 export default {
   data () {
     return {

     }
   },
   components: {

   },
   methods: {

   },
   mounted() {

   },
   watch: {

   },
   computed: {

   }
 }
</script>

<style scoped lang='scss'>
.col {
  display: flex;
  justify-content: center;
  width: 100%;
  height: 100px;
}
.logo {
      width: 150px;
      height: 80px;
      img {
        width: 100%;
        height: 100%;
      }
    }
.slogan {
  margin-top: 30px;
    font-size: 18px;
    color: #274a59;
    }
.nav-link-enterprise {
  color: #999;
  margin-top: 30px;
}
.nav-link {
  
  height: 15px;
  border: 1px solid #999;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 32px;
}

</style>