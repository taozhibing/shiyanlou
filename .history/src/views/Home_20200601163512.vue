<template>
 <div>
<navtitle></navtitle>
<nav :arr="arr"></nav>
 </div>
</template>

<script>
import Navtitle from '../components/home/Navtitle'
import Nav from '../components/home/Nav'
 export default {
   data () {
     return {
       arr : ''

     }
   },
   components: {
     Navtitle,
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