<template>
  <nav class="navbar navbar-dark navbar-expand-lg" style="background-color: rgba(0,140,160,0.6)">
    <div class="container">
      <a class="navbar-brand" href="https://wycode.cn" target="_self"><img src="https://wycode.cn/img/logo_48.png" width="32" height="32" alt="wycode.cn"> 王郁的小站</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="https://wycode.cn/blog/"><i class="fa fa-pencil fa-lg" aria-hidden="true"></i> 博客</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://wycode.cn/web/page/lab"><i class="fa fa-flask fa-lg" aria-hidden="true"></i> 实验室</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://wycode.cn/web/"><i class="fa fa-plug fa-lg" aria-hidden="true"></i> API</a>
          </li>
          <li class="nav-item">
            <a class="nav-link active" href="https://wycode.cn/vue/"><i class="fa fa-cog fa-lg" aria-hidden="true"></i> 后台</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://wycode.cn/android-docs/reference/packages.html"><i class="fa fa-android fa-lg" aria-hidden="true"></i> 安卓文档</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://wycode.cn/about.html"><i class="fa fa-user fa-lg" aria-hidden="true"></i> 关于</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>


<script>
  export default {
  }
</script>

<style scoped>
  .navbar-dark .navbar-nav .nav-link {
    color: #eee;
  }
  a.nav-link.active {
    background-color: rgba(0,140,160,0.8);
    border-radius: 4px;
  }
</style>
