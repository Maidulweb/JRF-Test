<script>
import Logo from "../assets/logo.png";
import ProfileLogo from "../assets/ProfileLogo.png";
export default {
  data: function () {
    return {
      Logo: Logo,
      ProfileLogo: ProfileLogo,
    };
  },
};
</script>

<template>
  <div class="main-navbar">
    <div class="container-fluid">
      <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
          <a class="navbar-brand logo" href="#"> <img :src="Logo" /></a>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <a class="nav-link active" aria-current="page" href="#">Home</a>
              </li>

              <li class="nav-item dropdown">
                <a
                  class="nav-link dropdown-toggle"
                  href="#"
                  role="button"
                  data-bs-toggle="dropdown"
                  aria-expanded="false"
                >
                  About Us
                </a>
                <ul class="dropdown-menu">
                  <li><a class="dropdown-item" href="#">Action</a></li>
                  <li><a class="dropdown-item" href="#">Another action</a></li>
                </ul>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">JRF Career Expo</a>
              </li>
              <li class="nav-item dropdown">
                <a
                  class="nav-link dropdown-toggle"
                  href="#"
                  role="button"
                  data-bs-toggle="dropdown"
                  aria-expanded="false"
                >
                  Career Support
                </a>
                <ul class="dropdown-menu">
                  <li><a class="dropdown-item" href="#">Action</a></li>
                  <li><a class="dropdown-item" href="#">Another action</a></li>
                </ul>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Faq</a>
              </li>
            </ul>
            <div class="notification-icon">
              <i class="fa-solid fa-bell"></i>
              <span class="notification-number">9</span>
            </div>
            <div class="profile-icon">
              <img :src="ProfileLogo" />
              <i class="fa-solid fa-angle-down"></i>
            </div>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<style>
.main-navbar {
  background-color: #fff;
}
.logo img {
  width: 140px;
}
.navbar-expand-lg .navbar-nav .nav-link {
  font-size: 14px;
  line-height: 19.36px;
  text-decoration: none;
  color: #000;
  padding-left: 15px;
}
.notification-icon {
  padding-left: 18px;
  position: relative;
}
.notification-number {
  position: absolute;
  right: -9px;
  top: -13px;
  background: red;
  padding: 0 3px;
  font-size: 11px;
  border-radius: 2px;
  color: #fff;
}
.profile-icon {
  padding-left: 18px;
}
.profile-icon img {
  width: 40px;
}
</style>
