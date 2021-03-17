<template>
  <div class="m-content">
    <h3>欢迎使用本校园论坛系统</h3>
    <div class="block">
      <el-avatar :size="50" :src="user.avatar"></el-avatar>
    </div>
    <div>
      <el-link href="/login" :underline="false">{{ user.username }}</el-link>
    </div>
    <div class="maction">
      <span>
        <el-link href="/blogs" type="primary" :underline="false">主页</el-link>
      </span>
      <el-divider direction="vertical"></el-divider>
      <span>
        <el-link href="/blog/add" type="success" :underline="false">发表文章</el-link>
      </span>
      <el-divider direction="vertical"></el-divider>
      <span>
        <el-link @click="logout" type="danger" :underline="false">退出账户</el-link>
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      user: {
        username: '请先登录',
        avatar: 'https://cube.elemecdn.com/3/7c/3ea6beec64369c2642b92c6726f1epng.png'
      }
    }
  },
  methods:{
    logout(){

    },
    login(){

    }
  }
}
</script>

<style scoped>
.m-content {
  margin: 0 auto;
  max-width: 960px;
  text-align: center;
}
.maction{
  margin: 10px auto;
}
</style>