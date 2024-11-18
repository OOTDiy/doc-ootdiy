<template>
  <v-footer :style="{ borderTop: '1px solid #ccc', height: '171px', width: '1280px' }">
    <v-row class="d-flex justify-space-between align-center" no-gutters>
      <!-- Kiri -->
      <v-col cols="6">
        <span>© 2025 SEAMEO QITEP in Science™. All Rights Reserved.</span>
      </v-col>

      <!-- Kanan (Link) -->
      <v-col class="d-flex justify-end" cols="6">
        <v-btn text to="/simulation">Simulation</v-btn>
        <v-btn text to="/teaching">Teaching</v-btn>
        <v-btn text to="/research">Research</v-btn>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
export default {
  name: "CustomFooter",
};
</script>

<style scoped>
/* Styling tambahan jika diperlukan */
</style>
