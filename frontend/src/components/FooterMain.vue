<script>
import FooterLogo from "../assets/footer logo.png";
export default {
  data: function () {
    return {
      FooterLogo: FooterLogo,
    };
  },
};
</script>
<template>
  <div class="footer">
    <div class="container-fluid">
      <div class="row d-flex flex-justify-between">
        <div class="col-md-4">
          <div class="footer-item">
            <img :src="FooterLogo" />
            <p>
              JRF Smart Job is a comprehensive job board website offering a
              range of services to both employers and job seekers. With job
              advertisements, recruiting services for global talents, specified
              skilled worker hiring solutions, and career fairs, JRF Smart Job
              connects businesses with top talent from around the world,
              providing a platform for successful hiring and career advancement.
            </p>
            <p>All Rights Reserved © 2023 JRFSmartJobs.com</p>
          </div>
        </div>
        <div class="col-md-2">
          <div class="footer-item">
            <h6>About Us</h6>
            <ul>
              <li>
                <a href="">Home</a>
              </li>
              <li>
                <a href="">About Us</a>
              </li>
              <li>
                <a href="">Company Profile</a>
              </li>
              <li>
                <a href="">Home</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-md-2">
          <div class="footer-item">
            <h6>About Us</h6>
            <ul>
              <li>
                <a href="">Home</a>
              </li>
              <li>
                <a href="">About Us</a>
              </li>
              <li>
                <a href="">Company Profile</a>
              </li>
              <li>
                <a href="">Home</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-md-2">
          <div class="footer-item">
            <h6>About Us</h6>
            <ul>
              <li>
                <a href="">Home</a>
              </li>
              <li>
                <a href="">About Us</a>
              </li>
              <li>
                <a href="">Company Profile</a>
              </li>
              <li>
                <a href="">Home</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-md-2">
          <div class="footer-item">
            <h6>About Us</h6>
            <ul>
              <li>
                <a href="">Home</a>
              </li>
              <li>
                <a href="">About Us</a>
              </li>
              <li>
                <a href="">Company Profile</a>
              </li>
              <li>
                <a href="">Home</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
.footer {
  background: #0b132e;
  padding: 20px;
}
.footer-item p {
  padding-top: 10px;
  color: #fff;
}
.footer-item h6 {
  color: #fff;
  padding-left: 30px;
  padding-top: 40px;
}
.footer-item ul li {
  list-style: none;
}
.footer-item ul li a {
  text-decoration: none;
  color: #fff;
  font-size: 12px;
  line-height: 19.36px;
}
</style>
