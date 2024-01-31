<script setup></script>

<template>
  <div class="left-sidebar">
    <ul class="list-unstyled ps-0">
      <li class="mb-3">
        <i class="fa-solid fa-house"></i>
        <a class="" href="">Home</a>
      </li>
      <li class="mb-3">
        <i class="fa-solid fa-table-columns"></i>
        <a class="" href="">Dashboard</a>
      </li>
      <li class="mb-3">
        <div class="d-flex">
          <i class="fa-solid fa-briefcase"></i>
          <button
            class="btn-toggle"
            data-bs-toggle="collapse"
            data-bs-target="#dashboard-collapse"
            aria-expanded="false"
          >
            Build Your Resume
          </button>
        </div>
        <div class="collapse" id="dashboard-collapse">
          <ul class="btn-toggle-nav list-unstyled fw-normal pb-1 small">
            <li><a href="#" class="link-dark rounded">New</a></li>
            <li><a href="#" class="link-dark rounded">Processed</a></li>
            <li><a href="#" class="link-dark rounded">Shipped</a></li>
            <li><a href="#" class="link-dark rounded">Returned</a></li>
          </ul>
        </div>
      </li>
      <li class="mb-3">
        <div class="d-flex">
          <i class="fa-solid fa-briefcase"></i>
          <button
            class="btn-toggle"
            data-bs-toggle="collapse"
            data-bs-target="#view-resume-collapse"
            aria-expanded="false"
          >
            View Resume
          </button>
        </div>
        <div class="collapse" id="view-resume-collapse">
          <ul class="btn-toggle-nav list-unstyled fw-normal pb-1 small">
            <li><a href="#" class="link-dark rounded">English Resume</a></li>
            <li><a href="#" class="link-dark rounded">Processed</a></li>
            <li><a href="#" class="link-dark rounded">Shipped</a></li>
          </ul>
        </div>
      </li>
      <li class="mb-3">
        <i class="fa-solid fa-house"></i>
        <a class="" href="">Message</a>
      </li>
      <li class="mb-3">
        <div class="d-flex">
          <i class="fa-solid fa-briefcase"></i>
          <button
            class="btn-toggle"
            data-bs-toggle="collapse"
            data-bs-target="#manage-job-collapse"
            aria-expanded="false"
          >
            Manage Job Application
          </button>
        </div>
        <div class="collapse" id="manage-job-collapse">
          <ul class="btn-toggle-nav list-unstyled fw-normal pb-1 small">
            <li><a href="#" class="link-dark rounded">English Resume</a></li>
            <li><a href="#" class="link-dark rounded">Processed</a></li>
            <li><a href="#" class="link-dark rounded">Shipped</a></li>
          </ul>
        </div>
      </li>
      <li class="mb-3">
        <i class="fa-solid fa-house"></i>
        <a class="" href="">Interview Schedules</a>
      </li>
      <li class="mb-3">
        <i class="fa-solid fa-house"></i>
        <a class="" href="">Following Employers</a>
      </li>
      <li class="mb-3">
        <i class="fa-solid fa-house"></i>
        <a class="" href="">Help & Support</a>
      </li>
      <li class="mb-3">
        <i class="fa-solid fa-house"></i>
        <a class="" href="">Setting</a>
      </li>
      <li class="mb-3">
        <i class="fa-solid fa-house"></i>
        <a class="" href="">Sign Out</a>
      </li>
    </ul>
  </div>
</template>

<style scoped>
.left-sidebar {
  padding-top: 30px;
  padding-left: 20px;
  background-color: #fff;
}

.left-sidebar ul li a {
  padding-left: 10px;
  font-size: 14px;
  text-decoration: none;
  color: #000;
  line-height: 19.36px;
}
.dropdown-toggle {
  outline: 0;
}

.nav-flush .nav-link {
  border-radius: 0;
}

.btn-toggle {
  display: inline-flex;
  padding-left: 10px;
  margin-top: -4px;
  color: #000;
  background-color: transparent;
  border: 0;
  font-size: 14px;
  line-height: 19.36px;
}
.btn-toggle:hover,
.btn-toggle:focus {
  color: #000;
}

.btn-toggle::after {
  width: 1em;
  line-height: 0;
  content: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='rgba%280,0,0,.5%29' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M5 14l6-6-6-6'/%3e%3c/svg%3e");
  transition: transform 0.35s ease;
  transform-origin: 0.5em 50%;
  margin-top: 4px;
  margin-left: 30px;
}

.btn-toggle[aria-expanded="true"] {
  color: rgba(0, 0, 0, 0.85);
}
.btn-toggle[aria-expanded="true"]::after {
  transform: rotate(90deg);
}

.btn-toggle-nav a {
  display: inline-flex;
  padding: 0.1875rem 0.5rem;
  margin-top: 0.125rem;
  margin-left: 1.25rem;
  text-decoration: none;
}
.btn-toggle-nav a:hover,
.btn-toggle-nav a:focus {
  background-color: #d2f4ea;
}

.scrollarea {
  overflow-y: auto;
}

.fw-semibold {
  font-weight: 600;
}
.lh-tight {
  line-height: 1.25;
}
</style>
