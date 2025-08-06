<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" temporary>
      Hello
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer" />
      <v-toolbar-title>My App</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <v-container>
        Main content
      </v-container>
    </v-main>
  </v-app>
</template>

<script setup>
import { ref } from 'vue'

const drawer = ref(false)
</script>
