<template>
  <v-card class="mx-auto overflow-hidden" width="100%" height="100%">
    <v-app-bar color="primary" dark>
      <v-app-bar-nav-icon @click="showMenu = true" />

      <v-toolbar-title>Title</v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer v-model="showMenu" absolute temporary>
      <v-list nav dense>
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <router-link :to="{ name: 'Main' }" class="text-decoration-none">
              <v-list-item-title>Home</v-list-item-title>
            </router-link>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </v-card>
</template>

<script>
export default {
  name: "HeaderComponent",

  data: () => ({
    showMenu: false,
    group: null,
  }),
};
</script>

<style scoped></style>
