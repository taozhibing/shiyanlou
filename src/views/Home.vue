<template>
 <div>
<navtitle></navtitle>
<navindex></navindex>
<nav></nav>
 </div>
</template>

<script>
import Navtitle from '../components/home/Navtitle'
import Nav from '../components/home/Nav'
import NavIndex from '../components/home/NavIndex'
 export default {
   data () {
     return {
       arr : ''

     }
   },
   components: {
     Navtitle,
     NavIndex,
     Nav

   },
   methods: {
     getClass(data) {
       this.arr = data
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