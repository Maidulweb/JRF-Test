<script setup>
import Information from "./Information.vue";
import LeftSidebar from "./LeftSidebar.vue";
</script>

<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-md-3">
        <LeftSidebar />
      </div>
      <div class="col-md-9">
        <div class="row">
          <div class="col-md-9">
            <div class="middle-body">
              <div class="information-slogan">
                <h4 class="mb-1">My Resume</h4>
                <p>Update your profile with your current status</p>
              </div>
              <div class="information">
                <Information />
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="progress blue">
              <span class="progress-left">
                <span class="progress-bar"></span>
              </span>
              <span class="progress-right">
                <span class="progress-bar"></span>
              </span>
              <div class="progress-value">
                <h6>90%</h6>
                <p>Profile Strength</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.information-slogan {
  padding-top: 30px;
}

.progress {
  width: 160px;
  height: 160px !important;
  line-height: 100px;
  background: none;
  margin: 0 auto;
  box-shadow: none;
  position: relative;
}
.progress:after {
  content: "";
  width: 100%;
  height: 100%;
  border-radius: 50%;
  border: 12px solid #fff;
  position: absolute;
  top: 0;
  left: 0;
}
.progress > span {
  width: 50%;
  height: 100%;
  overflow: hidden;
  position: absolute;
  top: 0;
  z-index: 1;
}
.progress .progress-left {
  left: 0;
}
.progress .progress-bar {
  width: 100%;
  height: 100%;
  background: none;
  border-width: 12px;
  border-style: solid;
  position: absolute;
  top: 0;
}
.progress .progress-left .progress-bar {
  left: 100%;
  border-top-right-radius: 80px;
  border-bottom-right-radius: 80px;
  border-left: 0;
  -webkit-transform-origin: center left;
  transform-origin: center left;
}
.progress .progress-right {
  right: 0;
}
.progress .progress-right .progress-bar {
  left: -100%;
  border-top-left-radius: 80px;
  border-bottom-left-radius: 80px;
  border-right: 0;
  -webkit-transform-origin: center right;
  transform-origin: center right;
  animation: loading-1 1.8s linear forwards;
}
.progress .progress-value {
  width: 90%;
  height: 90%;
  border-radius: 50%;
  background: #ffffff;
  position: relative;
}
.progress .progress-value h6 {
  position: absolute;
  color: red;
  top: 45%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.progress .progress-value p {
  position: absolute;
  color: red;
  top: 28%;
  left: 25%;
}
.progress.blue .progress-bar {
  border-color: #d10b4f;
}
.progress.blue .progress-left .progress-bar {
  animation: loading-2 1.5s linear forwards 1.8s;
}

@keyframes loading-1 {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(180deg);
    transform: rotate(180deg);
  }
}
@keyframes loading-2 {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(144deg);
    transform: rotate(144deg);
  }
}
@keyframes loading-3 {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(90deg);
    transform: rotate(90deg);
  }
}
@keyframes loading-4 {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(36deg);
    transform: rotate(36deg);
  }
}
@keyframes loading-5 {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(126deg);
    transform: rotate(126deg);
  }
}
@media only screen and (max-width: 990px) {
  .progress {
    margin-bottom: 20px;
  }
}
</style>
