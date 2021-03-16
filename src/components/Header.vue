<template>
  <div class="m-content">
    <h3>欢迎使用本论坛系统</h3>
    <div class="block">
      <el-avatar :size="50" :src="user.avatar"></el-avatar>
      <div>{{user.username}}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data(){
    return{
      user:{
        username:'请先登录',
        avatar:'https://cube.elemecdn.com/3/7c/3ea6beec64369c2642b92c6726f1epng.png'
      }
    }
  }
}
</script>

<style scoped>
.m-content{
  margin: 0 auto;
  max-width: 960px;
  text-align: center;
}
</style>