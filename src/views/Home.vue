<template>
 <div>
<div>
<navtitle></navtitle>
<nbv></nbv>
<ncv></ncv>
</div>
 </div>
</template>

<script>
import NavTitle from '../components/home/NavTitle'
import Nbv from '../components/home/Nbv'
import Ncv from '../components/home/Ncv'
 export default {
   data () {
     return {
       list:[]

     }
   },
   components: {
     NavTitle,
     Nbv,
     Ncv

   },
   methods: {
     getList(data) {
       this.list = data
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