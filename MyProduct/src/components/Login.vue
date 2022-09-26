<template>
  <div class="a">
    <div class="b" style="width:20%;margin: 0 auto">
      <el-input
        type="text"
        placeholder="请输入内容"
        v-model="text"
        maxlength="10"
        show-word-limit
        clearable
        center
      >
      </el-input>
      <div style="margin: 20px 0;"></div>
      <el-input
        placeholder="请输入密码"
        v-model="input"
        maxlength="30"
        show-word-limit
        show-password
        clearable
        center
      >
      </el-input>
      <div style="margin: 20px 0;"></div>
      <el-row>
        <el-button v-on:click="a">登入</el-button>
        <el-button v-on:click="b">注册</el-button>
      </el-row>
    </div>
  </div>


</template>

<script>
  export default {
    data() {
      return {
        input: '',
        text: ''
      }
    },
    methods:{
      a:function () {
        this.$router.push("/HelloWorld");
      },
      b:function () {
        this.$router.push("/register");
      }
    }
  }

</script>

<style scoped>
  .a{
    background: url("../imgs/1.png");
    height: 100%;
    width: 100%;
    position:fixed;
    background-size:100% 100%;
    blur:10px;
    margin: 0;
    overflow: hidden;
  }

</style>
