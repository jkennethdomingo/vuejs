<template>
  <div class="layout-wrapper layout-content-navbar">
      <div class="layout-container">
        <Menu />
        <div class="layout-page">
          <Sidebar />
            <div class="content-wrapper">
              <HelloWorld />
            </div>
        </div>
      </div>
      <div class="layout-overlay layout-menu-toggle"></div>
  </div>
</template>

<script>
import { defineComponent } from 'vue';

// Components
import HelloWorld from '../components/HelloWorld.vue';
import Sidebar from '@/components/Sidebar.vue';
import Menu from '../components/Menu.vue';

export default defineComponent({
  name: 'HomeView',

  components: {
    HelloWorld,
    Sidebar,
    Menu,
  },
});
</script>
