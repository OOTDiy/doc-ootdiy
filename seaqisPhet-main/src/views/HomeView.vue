<template>
  <v-container fluid class="pa-4">
  <HeroHome/>
   <ListCard />
  </v-container>
</template>

<script setup>
// Import the necessary Vuetify components
import { ref } from 'vue';
import ListCard from '@/components/layout/ListCard.vue';
import HeroHome from '@/components/common/HeroHome.vue';
</script>

<style scoped>
.v-card {
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.v-card-title {
  font-size: 18px;
  font-weight: bold;
  color: #333;
}

.v-card-subtitle {
  font-size: 14px;
  color: #555;
}

.v-btn {
  text-transform: none;
}

.v-row {
  margin-top: 20px;
}
</style>
