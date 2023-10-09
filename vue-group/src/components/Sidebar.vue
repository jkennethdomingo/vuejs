<template>
    <nav class="layout-navbar container-xxl navbar navbar-expand-xl navbar-detached align-items-center bg-navbar-theme" id="layout-navbar">
      <div class="layout-menu-toggle navbar-nav align-items-xl-center me-3 me-xl-0 d-xl-none">
        <a class="nav-item nav-link px-0 me-xl-4" href="#">
          <i class="bx bx-menu bx-sm"></i>
        </a>
      </div>
      
  
      <div class="navbar-nav-right d-flex align-items-center" id="navbar-collapse">
        <!-- Search -->
        <div class="navbar-nav align-items-center">
          <div class="nav-item d-flex align-items-center">
            <i class="bx bx-search fs-4 lh-0"></i>
            <input type="text" class="form-control border-0 shadow-none ps-1 ps-sm-2" placeholder="Search..." aria-label="Search..." />
          </div>
        </div>
        <!-- /Search -->
  
        <ul class="navbar-nav flex-row align-items-center ms-auto">
          <!-- User -->
          <li class="nav-item navbar-dropdown dropdown-user dropdown">
            <a class="nav-link dropdown-toggle hide-arrow" href="#" data-bs-toggle="dropdown">
              <div class="avatar avatar-online">
                <img src="/kcw.jpg" alt="User Avatar" class="w-px-40 h-auto rounded-circle" />
              </div>
            </a>
            <ul class="dropdown-menu dropdown-menu-end">
              <li>
                <a class="dropdown-item" href="#">
                  <div class="d-flex">
                    <div class="flex-shrink-0 me-3">
                      <div class="avatar avatar-online">
                        <img src="/kcw.jpg" alt="User Avatar" class="w-px-40 h-auto rounded-circle" />
                      </div>
                    </div>
                    <div class="flex-grow-1">
                      <span class="fw-medium d-block">Username</span>
                      <small class="text-muted">Admin</small>
                    </div>
                  </div>
                </a>
              </li>
              <li>
                <a class="dropdown-item" href="logout">
                  <i class="bx bx-power-off me-2"></i>
                  <span class="align-middle">Log Out</span>
                </a>
              </li>
            </ul>
          </li>
          <!--/ User -->
        </ul>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: "Sidebar",
};
  </script>
  
  <style scoped>
  @import '@/assets/assets/vendor/css/core.css';
  @import '@/assets/assets/vendor/css/theme-default.css';
  @import '@/assets/assets/css/demo.css';
  @import '@/assets/assets/vendor/libs/perfect-scrollbar/perfect-scrollbar.css';
  @import '@/assets/assets/vendor/libs/apex-charts/apex-charts.css';
  </style>
  