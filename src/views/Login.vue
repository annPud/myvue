<template>
  <div class="login-box">
    <el-row><el-col :span="8"></el-col>系统</el-row>
    <el-row>
      <el-col :span="8">
        <el-input id="name" v-model="name" placeholder="请输入帐号">
          <template slot="prepend">帐号</template>
        </el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="8">
        <el-input
          id="password"
          v-model="password"
          type="password"
          placeholder="请输入密码"
        >
          <template slot="prepend">密码</template>
        </el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="8">
        <el-button
          id="login"
          v-on:click="doLogin"
          style="width:100%"
          type="primary"
          >登录</el-button
        >
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
  methods: {
    doLogin: function(event) {
      console.log(event);
      console.log(this.data());
    },
    name: function() {}
  }
};
</script>
<style>
.el-row {
  margin-bottom: 20px;
}
.login-box {
  margin-top: 5%;
  margin-left: 40%;
}
</style>
