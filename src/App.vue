<template>
  <v-app>
    <HeaderComponent />
    <v-main>
      <router-view />
    </v-main>
    <FooterComponent />
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";
import HeaderComponent from "@/components/Header.vue";
import FooterComponent from "@/components/Footer.vue";

export default Vue.extend({
  name: "App",
  components: { FooterComponent, HeaderComponent },
  data: () => ({}),
});
</script>
