<template>
    <div class="login_container">
        <div class="login_box">
            <!-- 头像区 -->
            <div class="avatar_box">
                <img src="../assets/logo.png" alt="avatar">
            </div>
            <!-- 登陆表单 -->
            <div>
                <el-form ref="loginFormRef" :model="loginForm" label-width="60px">
                    <el-form-item label="账号">
                    <el-input v-model="loginForm.username"></el-input>
                    </el-form-item>
                </el-form>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  data () {
    return {
      loginForm: {
        username: 'admin',
        password: '123456'
      }
    }
  },
  methods () {

  }
}
</script>
<style lang="less" scoped>
.login_container {
      background-color: #2b4b6b;
      height: 100%;
}
.login_box {
    background-color: #ffffff;
    width: 450px;
    height: 360px;
  border-radius: 3px;
  position: absolute;
  left: 50%;
  top: 50%;
  -webkit-transform: translate(-50%, -50%);
  background-color: #fff;
}

.avatar_box {
        width: 130px;
    height: 130px;
    border: 1px solid #eee;
    border-radius: 50%;
    padding: 10px;
    box-shadow: 0 0 10px #ddd;
    position: absolute;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #fff;
    img {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      background-color: #eee;
    }
}
</style>
