<template>
    <div class="card">
      <h5 class="card-header">Manage Projects</h5>
      <div class="table-responsive text-nowrap">
        <table class="table table-hover">
          <thead>
            <tr>
              <th>Project</th>
              <th>Client</th>
              <th>Users</th>
              <th>Status</th>
              <th>Actions</th>
            </tr>
          </thead>
          <tbody class="table-border-bottom-0">
            <project-row v-for="(project, index) in projects" :key="index" :project="project" />
          </tbody>
        </table>
      </div>
    </div>
  </template>
  
  <script>
  import ProjectRow from './ProjectRow.vue';
  
  export default {
    components: {
      'project-row': ProjectRow,
    },
    data() {
      return {
        projects: [
          {
            name: 'Vuejs Project',
            iconClass: 'fab fa-angular fa-lg text-danger me-3',
            client: 'Dyze Malaluan',
            users: [
              { avatar: '/img/avatar-1.jpg', title: 'Kenneth' },
              { avatar: '/img/avatar-3.jpg', title: 'Jd' },
              { avatar: '/img/avatar-2.jpg', title: 'Ayen' },
            ],
            statusClass: 'badge bg-label-primary me-1',
            status: 'Active',
          },
           {
            name: 'CI4 Project',
            iconClass: 'fab fa-angular fa-lg text-danger me-3',
            client: 'Janine Santos',
            users: [
              { avatar: '/img/avatar-1.jpg', title: 'Kenneth' },
              { avatar: '/img/avatar-3.jpg', title: 'Jd' },
              { avatar: '/img/avatar-2.jpg', title: 'Ayen' },
            ],
            statusClass: 'badge bg-label-warning me-1',
            status: 'Pending',
          },
           {
            name: 'Python Project',
            iconClass: 'fab fa-angular fa-lg text-danger me-3',
            client: 'Krizza Bukid',
            users: [
              { avatar: '/img/avatar-1.jpg', title: 'Kenneth' },
              { avatar: '/img/avatar-3.jpg', title: 'Jd' },
              { avatar: '/img/avatar-2.jpg', title: 'Ayen' },
            ],
            statusClass: 'badge bg-label-success me-1',
            status: 'Completed',
          },
        ],
      };
    },
  };
  </script>

  