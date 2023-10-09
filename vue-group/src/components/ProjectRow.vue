<template>
    <tr>
      <td>
        <i :class="project.iconClass"></i>
        <span class="fw-medium">{{ project.name }}</span>
      </td>
      <td>{{ project.client }}</td>
      <td>
        <ul class="list-unstyled users-list m-0 avatar-group d-flex align-items-center">
          <li v-for="(user, userIndex) in project.users" :key="userIndex"
            data-bs-toggle="tooltip"
            data-popup="tooltip-custom"
            data-bs-placement="top"
            :title="user.title">
            <img :src="user.avatar" alt="Avatar" class="rounded-circle custom-image" />
          </li>
        </ul>
      </td>
      <td><span :class="project.statusClass">{{ project.status }}</span></td>
      <td>
        <div class="dropdown">
          <button type="button" class="btn p-0 dropdown-toggle hide-arrow" data-bs-toggle="dropdown">
            <i class="bx bx-dots-vertical-rounded"></i>
          </button>
          <div class="dropdown-menu">
            <a class="dropdown-item" href="javascript:void(0);"><i class="bx bx-edit-alt me-1"></i> Edit</a>
            <a class="dropdown-item" href="javascript:void(0);"><i class="bx bx-trash me-1"></i> Delete</a>
          </div>
        </div>
      </td>
    </tr>
  </template>
  
  <script>
  export default {
    props: {
      project: Object,
    },
  };
  </script>

<style scoped>

.custom-image {
      width: 2rem;
      height: 2rem;
      object-fit: cover;
    }
</style>
  