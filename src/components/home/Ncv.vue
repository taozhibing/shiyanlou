<template>
  <div>
    <div class="box"></div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  props: {},
  data() {
    return {
      list: []
    };
  },
  components: {},
  methods: {
    getData() {
      axios
        .get(" http://120.78.14.107/api/v2/index/categories")
        .then(res => {
          this.list = res.data.tags;
          this.$emit("getList", this.list);
        })
        .catch(err => {
          console.log(err);
        });
    }
  },
  mounted() {
    this.getData();
  },
  watch: {},
  computed: {}
};
</script>

<style scoped lang='scss'>

</style>