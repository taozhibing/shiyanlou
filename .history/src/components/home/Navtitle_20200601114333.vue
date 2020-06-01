<template>
 <div class="full-page">
<div class="col">
<div class="logo"><img src="https://static.shiyanlou.com/frontend/dist/img/9f43b00.svg" alt="实验楼" ></div>
</div>
<span class="slogan">做实验，学编程</span> 
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
    font-size: 18px;
    color: #274a59;
    }

</style>