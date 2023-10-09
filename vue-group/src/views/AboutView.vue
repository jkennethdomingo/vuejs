<template>
  <div class="layout-wrapper layout-content-navbar">
      <div class="layout-container">
        <Menu />
        <div class="layout-page">
          <Sidebar />
            <div class="content-wrapper">
              <div class="container-xxl flex-grow-1 container-p-y">
                <h4 class="py-3 mb-4"><span class="text-muted fw-light">Projects</span></h4>
                <Manage />
              </div>
            </div>
        </div>
      </div>
  </div>
</template>
<script>
import Sidebar from '@/components/Sidebar.vue';
import Menu from '@/components/Menu.vue';
import Manage from '@/components/Manage.vue';
export default {
name: 'AboutView',
components:{
    Sidebar,
    Menu,
    Manage,
}
}
</script>
<style>

</style>
