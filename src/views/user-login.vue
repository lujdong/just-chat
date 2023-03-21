<template>
  <div class="container">
    <el-card class="card-wrap">
      <h2 class="title">登录</h2>
      <el-form size="large">
        <el-form-item>
          <el-input placeholder="您的邮箱" clearable></el-input>
        </el-form-item>
        <el-form-item>
          <el-input type="password" placeholder="您的密码" clearable></el-input>
        </el-form-item>
        <el-form-item>
          <el-button type="primary" class="action-btn">登录</el-button>
        </el-form-item>
      </el-form>
      <p class="tip">还没有账号？去<el-button type="primary" link>注册</el-button></p>
    </el-card>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped lang="scss">
.container {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-image: linear-gradient(-225deg, #CBBACC 0%, #2580B3 100%);

  .title {
    letter-spacing: 10px;
    text-align: center;
  }

  .card-wrap {
    padding: 0 20px;

    .el-input {
      width: 320px;
      :deep(.el-input__inner:-webkit-autofill) {
        transition: background-color 50000s ease-in-out 0s;
      }
    }

    .action-btn {
      width: 100%;
    }

    .tip {
      display: flex;
      align-items: center;
      margin: 0;
      font-size: 14px;
    }
  }
}
</style>
