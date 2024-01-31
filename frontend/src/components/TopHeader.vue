<script setup></script>

<template>
  <div class="top-header">
    <div class="container-fluid">
      <div class="d-flex justify-content-between">
        <div class="header-left">
          <ul>
            <li><a href="">JOBS</a></li>
            <li><a href="">MY PAGE</a></li>
            <li><a href="">EMPLOYER SERVICES</a></li>
            <li><a class="post-a-job" href="">POST A JOB</a></li>
          </ul>
        </div>
        <div class="header-right">
          <div class="header-right-body d-flex">
            <a class="english" href="">ENG</a>
            <a class="japan" href="">日本語</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.top-header {
  background-color: #be1e2d;
  padding: 0 20px;
}
.header-left ul {
  padding: 0;
  margin: 0;
}
.header-left ul li {
  display: inline-block;
  padding: 10px 18px 10px 0;
}
.header-left ul li a {
  font-size: 12px;
  line-height: 19.36px;
  text-decoration: none;
  color: #ffffff;
}
.post-a-job {
  border: 1px solid #fff;
  padding: 4px 8px;
  border-radius: 8px;
}
.header-right-body {
  height: 27px;
  margin-top: 8px;
}
.header-right-body a {
  font-size: 12px;
  line-height: 19.36px;
  text-decoration: none;
  color: #222;
  padding: 4px;
}
.header-right-body .english {
  background-color: #fff;
  border-radius: 4px 0px 0 4px;
}
.header-right-body .japan {
  background-color: #9e9d9d;
  border-radius: 0 4px 4px 0;
}
</style>
