<template>
  <v-app>
    <VNavigationDrawer v-model:model-value="drawer" expand-on-hover="" rail="" temporary="">
      <VList>
          <VListItem
            prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
            subtitle="sandra_a88@gmailcom"
            title="Sandra Adams"
          ></VListItem>
       </VList>
    </VNavigationDrawer>

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
import { VList, VListItem, VNavigationDrawer } from 'vuetify/lib/components';

const drawer = ref(false)
</script>
