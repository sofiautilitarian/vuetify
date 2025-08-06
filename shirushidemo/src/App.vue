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
import ImageGallery from './components/ImageGallery.vue';
import SideBar from './components/SideBar.vue';

export default {
  components: {
    SideBar,
    ImageGallery
  },
  data() {
    return {
      drawer: false,
    };
  },
};
</script>
