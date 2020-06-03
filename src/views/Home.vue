<template>
 <div>
<div>
<navtitle></navtitle>
<nbv></nbv>
<ncv></ncv>
<ndv></ndv>
</div>
 </div>
</template>

<script>
import Navtitle from '../components/home/Navtitle'
import Nbv from '../components/home/Nbv'
import Ncv from '../components/home/Ncv'
import Ndv from '../components/home/Ndv'
 export default {
   data () {
     return {
       list:[],
       arr : []

     }
   },
   components: {
     Navtitle,
     Nbv,
     Ncv,
     Ndv

   },
   methods: {
     getList(data) {
       this.list = data
     },
     getArr(data) {
       this.arr = data
     },
     getArr1(data) {
       this.arr1 = data
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