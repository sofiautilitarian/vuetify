<template>
    <VApp>
        <VNavigationDrawer v-model:model-value="drawer" expand-on-hover="" rail="" temporary="">
            <VList>
                <VListItem prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
                    subtitle="sandra_a88@gmailcom" title="Sandra Adams"></VListItem>
            </VList>

            <VDivider />
            <VList density="compact" nav>
                <VListItem prepend-icon="mdi-dialpod" title="Grayspace Gallery" value='color'></VListItem>

            
            </VList>
        </VNavigationDrawer>




        <v-app-bar app>
            <v-app-bar-nav-icon @click="drawer = !drawer" />
            <v-toolbar-title>My App</v-toolbar-title>
        </v-app-bar>

        <v-main>
            <v-container>
                <ImageGallery/>
            </v-container>
        </v-main>
    </VApp>
</template>

<script setup>
import { ref } from 'vue'
import { VList, VListItem, VNavigationDrawer } from 'vuetify/lib/components';
import ImageGallery from './ImageGallery.vue';

const drawer = ref(false)
</script>
