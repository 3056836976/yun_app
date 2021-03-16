<template>
  <div>
    <el-container>
      <el-header>
        <img class="logo" src="../assets/logo.png">
      </el-header>
      <el-main>
        <el-form :model="ruleForm" :rules="rules" ref="ruleForm" label-width="100px" class="demo-ruleForm">
          <el-form-item label="用户名" prop="name">
            <el-input v-model="ruleForm.name" placeholder="请输入用户名"></el-input>
          </el-form-item>

          <el-form-item label="密码" prop="password">
            <el-input v-model="ruleForm.password" placeholder="请输入密码" show-password></el-input>
          </el-form-item>

          <el-form-item  label="验证码" prop="my_check" class="check_code">
            <el-input v-model="ruleForm.check" placeholder="请输入验证码" class="check_code"></el-input>

          </el-form-item>

          <el-form-item class="sure">
            <el-button type="primary" @click="login()">登录</el-button>
            <el-button @click="resetForm('ruleForm')">重置</el-button>
          </el-form-item>

          <div class="mor">
            <span>
              <el-link @click="reg" type="primary" :underline="false">注册帐户</el-link>
            </span>
            <el-divider direction="vertical"></el-divider>
            <span>
              <el-link @click="forget" type="success" :underline="false">忘记密码</el-link>
            </span>
          </div>
        </el-form>
      </el-main>
    </el-container>
  </div>
</template>

<script>

export default {
  name: "Login",
  data() {
    return {
      ruleForm: {
        name: '',
        password: '',
        region: ''
      },
      rules: {
        name: [
          {required: true, message: '请输入用户名', trigger: 'blur'},
          {min: 3, max: 8, message: '长度在 3 到 8个字符', trigger: 'blur'}
        ],
        password: [
          {required: true, message: '请输入密码', trigger: 'blur'},
          {min: 8, message: '密码长度不少于8个字符', trigger: 'blur'}
        ],
        my_check:[
          {required: true, message:'请输入验证码', trigger: 'blur'}
        ]
      }
    };
  },
  methods: {
    login() {

    },
    reg() {

    },
    forget() {

    },
    resetForm(formName) {
      this.$refs[formName].resetFields();
    }
  }
}
</script>

<style scoped>
.el-header, .el-footer {
  background-color: #B3C0D1;
  color: #333;
  text-align: center;
  line-height: 60px;
}

.el-aside {
  background-color: #D3DCE6;
  color: #333;
  text-align: center;
  line-height: 200px;
}

.el-main {
  /*background-color: #E9EEF3;*/
  color: #333;
  text-align: center;
  line-height: 0px;
}

.el-option {
  max-width: 50px;
}

body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}


.logo {
  height: 60%;
  margin-top: 15px;
}

.demo-ruleForm {
  margin: 0 auto;
  margin-top: 50px;
  max-width: 500px;

}

.check_code{
  width: 180px;
}

.sure {
  max-width: 250px;
}

.mor {
 width: 330px;

}
</style>


