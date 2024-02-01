<script setup>
import LeftSidebar from "./LeftSidebar.vue";
import Information from "./Information.vue";
</script>

<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-md-3">
        <LeftSidebar />
      </div>
      <div class="col-md-9">
        <div class="information-slogan">
          <h4 class="mb-1">My Resume</h4>
          <p>Update your profile with your current status</p>
        </div>
        <div class="row">
          <div class="col-md-9">
            <div class="middle-body">
              <div class="information">
                <Information />
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="profile-progress">
              <div class="progress-n blue">
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
              <div class="profile-progress-report">
                <div class="d-flex">
                  <i class="fa-solid fa-check"></i>
                  <p class="">Basic Information (15%)</p>
                </div>
                <div class="d-flex">
                  <i class="fa-solid fa-check"></i>
                  <p class="">Education (20%)</p>
                </div>
                <div class="d-flex">
                  <i class="fa-solid fa-check"></i>
                  <p class="">Skills & Language (35%)</p>
                </div>
                <div class="d-flex">
                  <i class="fa-solid fa-check"></i>
                  <p class="">Work History (15%)</p>
                </div>
                <div class="d-flex">
                  <i class="fa-solid fa-check"></i>
                  <p class="">Portfolios & Certifications (10%)</p>
                </div>
                <div class="d-flex">
                  <i class="fa-solid fa-check"></i>
                  <p class="">References 5%</p>
                </div>
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
.profile-progress {
  margin-top: 30px;
  background-color: #fff;
  padding-top: 10px;
  border-radius: 8px;
}
.progress-n {
  width: 160px;
  height: 160px !important;
  line-height: 100px;
  background: transparent;
  margin: 0 auto;
  box-shadow: none;
  position: relative;
}
.progress-n:after {
  content: "";
  width: 100%;
  height: 100%;
  border-radius: 50%;
  border: 0;
  position: absolute;
  top: 0;
  left: 0;
}
.progress-n > span {
  width: 50%;
  height: 100%;
  overflow: hidden;
  position: absolute;
  top: 0;
  z-index: 1;
}
.progress-n .progress-left {
  left: 0;
}
.progress-n .progress-bar {
  width: 100%;
  height: 100%;
  background: transparent;
  border-width: 12px;
  border-style: solid;
  position: absolute;
  top: 0;
  color: #3ab446;
}

.progress-n .progress-left .progress-bar {
  left: 100%;
  border-top-right-radius: 80px;
  border-bottom-right-radius: 80px;
  border-left: 0;
  -webkit-transform-origin: center left;
  transform-origin: center left;
}
.progress-n .progress-right {
  right: 0;
}
.progress-n .progress-right .progress-bar {
  left: -100%;
  border-top-left-radius: 80px;
  border-bottom-left-radius: 80px;
  border-right: 0;
  -webkit-transform-origin: center right;
  transform-origin: center right;
  animation: loading-1 1.8s linear forwards;
}
.progress-n .progress-value {
  width: 90%;
  height: 90%;
  border-radius: 50%;
  background: transparent;
  position: relative;
}
.progress-n .progress-value h6 {
  position: absolute;
  color: #3ab446;
  top: 45%;
  left: 55%;
  transform: translate(-50%, -50%);
  font-size: 30px;
  font-weight: 900;
}
.progress-n .progress-value p {
  position: absolute;
  color: #000;
  top: 58%;
  left: 21%;
}
.progress.blue .progress-bar {
  border-color: #d10b4f;
}
.progress-n.blue .progress-left .progress-bar {
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
.profile-progress-report p {
  padding-left: 10px;
}
.profile-progress-report {
  padding-top: 10px;
}
.profile-progress-report i {
  background: #3ab446;
  border-radius: 50%;
  width: 20px;
  height: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #fff;
  font-size: 9px;
}
</style>
