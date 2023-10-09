<template>
  <v-container class="my-5">
    <v-subheader class="custom-subheader">Our Team</v-subheader>
    <v-row>
      <v-col cols="12" sm="6" md="4" lg="3" v-for="person in team" :key="person.name">
        <v-card class="custom-card">
          <v-responsive class="pt-4 custom-avatar">
            <v-avatar size="100" class="grey lighten-2 ml-3">
              <img :src="person.avatar" class="custom-image">
            </v-avatar>
          </v-responsive>
          <v-card-text class="text-center">
            <div class="subheading">{{ person.name }}</div>
            <div class="grey--text">{{ person.role }}</div>
          </v-card-text>
          <v-card-actions class="text-center">
            <v-btn flat color="grey" class="text-center">
              <v-icon small left>message</v-icon>
              <span class="">Message</span>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      team: [
        { name: 'Kenneth', role: 'Web developer', avatar: '/img/avatar-1.jpg' },
        { name: 'Jd', role: 'Graphic designer', avatar: '/img/avatar-3.jpg' },
        { name: 'Ayen', role: 'Web developer', avatar: '/img/avatar-2.jpg' },
      ]
    };
  }
};
</script>

<style scoped>
.custom-subheader {
  font-size: 1.5rem;
}

.custom-card {
  border: 1px solid #ccc;
  margin: 1rem;
  padding: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.custom-avatar {
  display: flex;
  justify-content: center;
  align-items: center;
}

.custom-image {
  width: 6.25rem;
  height: 6.25rem;
  object-fit: cover;
}
</style>
