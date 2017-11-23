<template>
  <div class="container">
    <div class="row">

      <form class="form-signup col-5 offset-3">
        <h2 class="form-signup-heading">注册</h2>
        <input type="text" id="inputUser" class="form-control" placeholder="用户名*" required="" autofocus="">
        <input type="tel" id="inputPhone" class="form-control" placeholder="手机号" required="">
        <input type="password" id="inputPassword" class="form-control" placeholder="密码*" required="">
        <button class="btn btn-primary btn-block" type="submit">注册</button>
        <router-link to="/login" class ="login">已有账号？立即登录</router-link>
      </form>
    </div>
  </div>
</template>


<script>
  export default {
    name: 'Register'
  }
</script>


<style scoped>

  .form-signup-heading{
    text-align: center;
    margin-bottom: 12px;
  }

  .login{
    margin-top: 12px;
    font-size: 12px;
  }

  .row {
    margin-top: 32px;
  }

  input,button{
    margin-top: 6px;
  }

  .form-signup {
    background-color: #eef;
    padding: 16px;
    border: 1px solid #c2cfd6;
    border-radius: 4px;
  }
</style>
