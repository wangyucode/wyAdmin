<template>
  <div class="container">
    <div class="row">

      <div class="tech-stack col-6">
        <h2>技术栈</h2>
        <ul>
          <li>Bootstrap</li>
          <li>Vue</li>
          <li>Vue Router</li>
          <li>Vuex</li>
          <li>Axios</li>
          <li>Spring Boot</li>
          <li>Spring Security</li>
          <li>Spring JPA</li>
          <li>Thymeleaf</li>
          <li>H2 Database</li>
          <li>Swagger</li>
          <li>JWT</li>
        </ul>
      </div>

      <form class="form-signin col-4 offset-2">
        <h2 class="form-signin-heading">登录</h2>
        <p class="text-info">可以使用guest guest 游客登录</p>
        <input type="text" id="inputUser" class="form-control" placeholder="用户名" required="" autofocus="" v-model="loginForm.username">
        <input type="password" id="inputPassword" class="form-control" placeholder="密码" required="" v-model="loginForm.password">
        <button class="btn btn-primary btn-block" type="submit" v-on:click="handleLogin">登录</button>
        <p class="text-danger" v-if="isShowError">{{message}}</p>
        <br/>
        <router-link to="/register" class="register">没有账号？立即注册</router-link>
      </form>

    </div>
  </div>
</template>


<script>
  export default {
    name: 'Login',
    data() {
      return {
        loginForm: {
          username: '',
          password: ''
        },
        message: '',
        isShowError: false
      }
    },
    methods: {
      handleLogin: function () {
        // `this` 在方法里指向当前 Vue 实例
        this.$store.dispatch('Login',this.loginForm).then(()=>{
          this.$router.push({path:'/'})
        })
      }
    }
  }
</script>


<style scoped>

  .form-signin-heading {
    text-align: center;
    margin-bottom: 12px;
  }

  .register {
    margin-top: 12px;
    font-size: 12px;
  }

  .row {
    margin-top: 32px;
  }

  input, button {
    margin-top: 6px;
  }

  .form-signin {
    background-color: #eef;
    padding: 16px;
    border: 1px solid #c2cfd6;
    border-radius: 4px;
  }
</style>
