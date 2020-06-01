<template>
  <div class="full-page">
    <div class="col">
      <div class="logo">
        <img src="https://static.shiyanlou.com/frontend/dist/img/9f43b00.svg" alt="实验楼" />
      </div>
      <span class="slogan">做实验，学编程</span>
      <div style="width:500px;height:100px"></div>
      <a href="" class="nav-link-enterprise">企业版</a>
      <span class="nav-link"></span>
      <a href="" class="nav-link-enterprise">学校版</a>
      <a href="" class="nav-click"> 登录</a>
      <div class="nav-register">
        <div class="register">注册</div>
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
  methods: {
  },
  mounted() {},
  watch: {},
  computed: {}
};
</script>

<style scoped lang='scss'>
.col {
  display: flex;
  justify-content: center;
  width: 100%;
  height: 100px;
}
.logo {
  width: 150px;
  height: 80px;
  img {
    width: 100%;
    height: 100%;
  }
}
.slogan {
  margin-top: 30px;
  font-size: 18px;
  color: #274a59;
}
.nav-link-enterprise {
  color: #999;
  margin-top: 30px;
  text-decoration: none;
}
.nav-link-enterprise:hover {
  color: #08bf91;
}
.nav-link {
  height: 15px;
  border: 1px solid #999;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 32px;
}
.nav-click {
  margin-left: 30px;
  margin-top: 30px;
  color: #08bf91;
}
.nav-register {
  display: flex;
  align-content: center;
  justify-content: center;
  width: 80px;
  height: 50px;
  background: #08bf91;
  margin-top: 15px;
  margin-left: 20px;
  .register {
    color: #fff;
    margin-top: 15px;
  }
}
</style>