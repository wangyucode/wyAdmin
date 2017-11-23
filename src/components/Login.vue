<template>
  <div class="container">
    <div class="row">

      <div class="tech-stack col-6">
        <h2>技术栈</h2>
        <ul>
          <li>1234</li>
          <li>1234</li>
          <li>1234</li>
          <li>1234</li>
        </ul>
      </div>

      <form class="form-signin col-4 offset-2">
        <h2 class="form-signin-heading">登录</h2>
        <p class="text-info">可以使用guest guest 游客登录</p>
        <input type="text" id="inputUser" class="form-control" placeholder="用户名" required="" autofocus="">
        <input type="password" id="inputPassword" class="form-control" placeholder="密码" required="">
        <button class="btn btn-primary btn-block" type="submit">登录</button>
        <router-link to="/register" class ="register">没有账号？立即注册</router-link>
      </form>

    </div>
  </div>
</template>


<script>
  export default {
    name: 'Login'
  }
</script>


<style scoped>

  .form-signin-heading{
    text-align: center;
    margin-bottom: 12px;
  }

  .register{
    margin-top: 12px;
    font-size: 12px;
  }

  .row {
    margin-top: 32px;
  }

  input,button{
    margin-top: 6px;
  }

  .form-signin {
    background-color: #eef;
    padding: 16px;
    border: 1px solid #c2cfd6;
    border-radius: 4px;
  }
</style>
