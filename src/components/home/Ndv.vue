<template>
  <div>
    <div class="box">
      <div class="nav">
        <div class="top">
          <div class="t-left">
            <div class="t-font">精选项目课</div>
            <a class="t-font2" href>精选会员项目课程,动手中收获</a>
          </div>
          <div class="t-right">
            <a href>更多>></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      arr1: []
    };
  },
  components: {},
  methods: {
    getData() {
      axios
        .get("//120.78.14.107/api/v2/index/classfication-courses")
        .then(res => {
          this.arr1 = res.data;
          this.$emit("getArr1", this.arr1);
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
.box {
  width: 100%;
  display: flex;
  justify-content: center;
  margin-top: 10px;
}
.nav {
  width: 1180px;
}
.top {
  display: flex;
  justify-content: space-between;
}
.t-left {
  height: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.t-font {
  font-weight: 700;
  font-size: 24px;
}
.t-font2 {
  border-left: 2px solid black;
  margin-left: 10px;
  padding-left: 10px;
}
a {
  text-decoration: none;
  color: black;
}
.t-right {
  height: 80px;
  display: flex;
  align-items: center;
}
</style>