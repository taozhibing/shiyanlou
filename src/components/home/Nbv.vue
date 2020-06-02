<template>
  <div>
    <div class="box">
      <div class="mildle">
        <div class="left">
          <div class="l-item">
            <div class="item">
              <a class="item-a" href>后端开发</a>
              <a class="item-a" href>Python</a>
              <a class="item-a" href>PHP</a>
            </div>
            <div class="item-b">
              <div class="itemb-1">后端开发</div>
              <div class="itemb-2">
                <a class="itemb-3">Python</a>
                <a class="itemb-3">Python</a>
              </div>
              <div class="itemb-1">课程推荐</div>
            </div>
          </div>
          <div class="l-item">
            <div class="item">
              <a class="item-a" href>Linux运维</a>
              <a class="item-a" href>Linux</a>
              <a class="item-a" href>Shell</a>
            </div>
            <div class="item-b">
              <div class="itemb-1">Linux运维</div>
              <div class="itemb-2">
                <a class="itemb-3">Python</a>
                <a class="itemb-3">Python</a>
              </div>
              <div class="itemb-1">课程推荐</div>
            </div>
          </div>
          <div class="l-item">
            <div class="item">
              <a class="item-a" href>云计算与大数据</a>
              <a class="item-a" href>Hadoop</a>
              <a class="item-a" href>Spark</a>
            </div>
            <div class="item-b">
              <div class="itemb-1">云计算与大数据</div>
              <div class="itemb-2">
                <a class="itemb-3">Python</a>
                <a class="itemb-3">Python</a>
              </div>
              <div class="itemb-1">课程推荐</div>
            </div>
          </div>
           <div class="l-item">
            <div class="item">
              <a class="item-a" href>数据库</a>
              <a class="item-a" href>SQL</a>
              <a class="item-a" href>NoSQL</a>
            </div>
            <div class="item-b">
              <div class="itemb-1">数据库</div>
              <div class="itemb-2">
                <a class="itemb-3">SQL</a>
                <a class="itemb-3">NoSQL</a>
              </div>
              <div class="itemb-1">课程推荐</div>
            </div>
          </div>
              <div class="l-item">
            <div class="item">
              <a class="item-a" href>信息安全</a>
              <a class="item-a" href>Web安全</a>
              <a class="item-a" href>安全开发</a>
            </div>
            <div class="item-b">
              <div class="itemb-1">信息安全</div>
              <div class="itemb-2">
                <a class="itemb-3">Web安全</a>
                <a class="itemb-3">安全开发</a>
              </div>
              <div class="itemb-1">课程推荐</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  props: {},
  data() {
    return {
      list:[]
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

<style scoped>
.box {
  width: 100%;
  display: flex;
  justify-content: center;
  background: rgb(255, 204, 51);
  height: 515px;
}
.mildle {
  width: 1200px;
  padding-left: 10px;
  height: 100%;
  background: chocolate;
}
.left {
  width: 260px;
  background: rgba(0, 0, 0, 0.18);
  margin-left: 5px;
}
.l-item {
  display: flex;
  justify-content: center;
  position: relative;
}
.l-item:hover {
  background: white;
}
.l-item:hover .item-b {
  visibility: visible;
}
.item:hover .item-a {
  color: #666;
}
.item {
  display: flex;
  width: 240px;
  height: 50px;
  align-items: center;
  justify-content: space-around;
  border-bottom: 1px solid white;
}
.item-a {
  color: white;
}
.item-a:hover {
  color: #08bf91 !important;
}
a {
  text-decoration: none;
}
.item-b {
  width: 300px;
  height: 300px;
  position: absolute;
  background: white;
  top: 0;
  left: 260px;
  visibility: hidden;
}
.itemb-1 {
  margin-left: 20px;
  width: 100px;
  height: 30px;
  background: rgb(238, 238, 238);
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10px;
  font-size: 14px;
}
.itemb-2 {
  margin-left: 20px;
  margin-top: 10px;
  display: flex;
}

.itemb-3 {
  color: black;
  border-left: 1px solid black;
  padding: 2px;
}
.itemb-3:hover {
  color: #08bf91;
}
</style>