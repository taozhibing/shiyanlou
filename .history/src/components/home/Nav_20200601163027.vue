<template>
 <div>

 </div>
</template>

<script>
import axios from 'axios'
 export default {
   data () {
     return {
       arr : ''

     }
   },
   components: {

   },
   methods: {
     getData() {
       axios.get(`http://120.78.14.107/api/v2/index/categories`).then(res => {
         this.arr = res.data
         this.$emit('getClass',this.arr)

       }).catch(err => {
         console.log(err)
       })
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