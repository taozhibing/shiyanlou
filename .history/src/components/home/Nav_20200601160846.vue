<template>
 <div>

 </div>
</template>

<script>
import axios from 'axios'
 export default {
   data () {
     return {

     }
   },
   components: {

   },
   methods: {
     getData() {
       axios.get(`http://120.78.14.107/api/v2/index/categories`)
     }

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

</style>