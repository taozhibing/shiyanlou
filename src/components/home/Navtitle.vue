<template>
  <div>
    <div class="box">
      <div class="nava">
        <div class="n-top">
          <div class="n-right">
            <div>
              <img
                src="https://static.shiyanlou.com/frontend/dist/img/9f43b00.svg"
                alt
                width="122px"
                height="50px"
              />
            </div>
            <span class="item">做实验，学编程</span>
          </div>
          <div class="n-left">
            <a href>
              <div class="nl">企业版</div>
            </a>
            <div class="nl-1"></div>
            <a href>
              <div class="nl">学校版</div>
            </a>
            <a href>
              <div class="nl-3">登陆</div>
            </a>
            <a href>
              <div class="nl-2">注册</div>
            </a>
          </div>
        </div>
        <div class="n-foot">
          <div class="nf1">
            <div class="nf2">
              <img src="../home/pic/1.png" alt />
              <a class="anf" href>全部课程</a>
            </div>
          </div>
          <div class="nf3">
            <div class="nf4">
              <a class="nl" href>路径</a>
              <a class="nl" href>训练营</a>
              <a class="nl" href>楼+</a>
              <a class="nl nlb" href>
                会员
                <img
                  src="https://static.shiyanlou.com/frontend/dist/img/02a4001.svg"
                  alt
                  class="nlc"
                />
              </a>
              <a class="nl" href>
                社区
                <img src="../home/pic/3.png" alt />
                <div class="nla">
                  <a href>讨论</a>
                  <a href>教程库</a>
                  <a href>直播</a>
                  <a href>比赛</a>
                </div>
              </a>
            </div>
            <div class="nf5 nl">
              <div>
                <input type="text" placeholder="搜索 课程/问答" class="ipt" />
              </div>
              <div class="nf6">
                <img src="../home/pic/2.png" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  components: {},
  methods: {},
  mounted() {},
  watch: {},
  computed: {}
};
</script>

<style scoped>
a {
  text-decoration: none;
  color: #333333;
}

.box {
  width: 100%;
  height: 150px;
  background: rgb(249, 249, 249);
  display: flex;
  justify-content: center;
}
.nava {
  width: 1200px;
}
.n-top {
  width: 1180px;
  height: 65px;
  display: flex;
  justify-content: space-between;
  padding: 10px;
}
.n-right {
  width: 300px;
  display: flex;
  align-items: center;
}
.n-left {
  display: flex;
  justify-content: space-around;
  width: 285px;
  align-items: center;
}
.nl-1 {
  width: 2px;
  height: 20px;
  background: rgb(153, 153, 153);
}
.nl-2 {
  height: 50px;
  width: 50px;
  background: rgb(8, 191, 145);
  display: flex;
  align-items: center;
  color: white;
  justify-content: center;
}
.item {
  height: 50px;
  display: flex;
  align-items: center;
}
.nl {
  position: relative;
}
.nla {
  position: absolute;
  left: -10px;
  width: 150px;
  background: white;
  top: 20px;
  visibility: hidden;
  border-radius: 5px;
  box-shadow: 0 15px 16px 0 rgba(0, 0, 0, 0.18);
}
.nl:hover .nla {
  visibility: visible;
}
.nl:hover {
  color: #08bf91;
}
.nla a {
  display: flex;
  height: 50px;
  align-items: center;
  padding-left: 10px;
}
.nla a:hover {
  color: #08bf91;
  background: #f7f7f7;
}
.nl-3 {
  color: #08bf91;
}
.nl-3:hover {
  color: black;
}
.n-foot {
  width: 1180px;
  height: 55px;
  display: flex;
  align-items: center;
  padding: 10px;
  background: white;
}
.nf1 {
  width: 260px;
  height: 55px;
  background: rgb(84, 193, 133);
  display: flex;
  align-items: center;
}
.anf {
  color: white;
}
.nf2 {
  padding-left: 15px;
  display: flex;
  align-items: center;
}
.nf3 {
  width: 880px;
  display: flex;
  justify-content: space-between;
}
.nf4 {
  width: 350px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.nf5 {
  width: 210px;
  height: 30px;
  border: 1px solid rgb(231, 234, 237);
  border-radius: 5px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.nf5:hover {
  border-color: #08bf91;
}
.nf6 {
  width: 34px;
  height: 29px;
}
.ipt {
  border: none;
  outline: none;
  padding-left: 5px;
  width: 130px;
}
.nlb {
  position: relative;
}
.nlc {
  position: absolute;
  bottom: 20px;
  left: 30px;
}
</style>