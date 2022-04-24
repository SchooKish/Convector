<template>
  <v-footer fixed padless>
    <v-card width="100%" class="primary text-center">
      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} - <strong>SchooKish</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style scoped></style>
