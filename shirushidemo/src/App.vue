<template>
  <v-app>
    <!-- Sidebar component -->
    <SideBar />

    <!-- Main content -->
    <v-main>
      <v-container>
        <v-card class="pa-4">
          <v-navigation-drawer
            v-model="drawer"
            expand-on-hover
            rail
            temporary
          >
            <v-list>
              <v-list-item>
                Hello from drawer!
              </v-list-item>
            </v-list>
          </v-navigation-drawer>
        </v-card>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import SideBar from './components/SideBar.vue';

export default {
  components: {
    SideBar,
  },
  data() {
    return {
      drawer: false,
    };
  },
};
</script>
