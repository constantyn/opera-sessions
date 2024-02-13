<template>
  <v-app>
    <v-layout>
      <v-app-bar title="Opera Sessions">
        <template #append>
          <v-app-bar-nav-icon @click="drawerOpen = !drawerOpen" />
        </template>
      </v-app-bar>

      <v-navigation-drawer v-model="drawerOpen" location="end">
        <v-list>
          <v-list-item title="Home" />
        </v-list>
      </v-navigation-drawer>

      <v-main>
        <v-sheet class="ma-6">
          <v-alert type="info">Hello world!</v-alert>
        </v-sheet>
      </v-main>
    </v-layout>
  </v-app>
</template>

<script lang="ts" setup>
const drawerOpen = ref(false);
</script>
