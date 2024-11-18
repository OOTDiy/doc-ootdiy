<template>
  <div>
    <!-- Section Chemistry -->
    <div>
      <div class="title-container">
        <h1 class="section-title">Biology</h1>
        <v-btn text @click="toggleChemistry" class="show-more-btn">
          Show More
          <v-icon>{{ showBiology ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
        </v-btn>
      </div>
      <img src="@/assets/fotoSimulasi/seaqistanam.svg" width="173px" height="206px" alt=""/>
      <v-collapse v-if="showBiology">
        <!-- Additional content for Biology -->
        <p>Details about Biology simulation...</p>
      </v-collapse>
    </div>

    <!-- Section Physics -->
    <div>
      <div class="title-container">
        <h1 class="section-title">Physics</h1>
        <v-btn text @click="togglePhysics" class="show-more-btn">
          Show More
          <v-icon>{{ showPhysics ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
        </v-btn>
      </div>
      <img src="@/assets/fotoSimulasi/seaqiselektro.svg" width="173px" height="206px" alt=""/>
      <v-collapse v-if="showPhysics">
        <!-- Additional content for Physics -->
        <p>Details about Physics simulation...</p>
      </v-collapse>
    </div>

    <!-- Section Biology -->
    <div>
      <div class="title-container">
        <h1 class="section-title">Chemistry</h1>
        <v-btn text @click="toggleBiology" class="show-more-btn">
          Show More
          <v-icon>{{ showChemistry ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
        </v-btn>
      </div>
      <img src="@/assets/fotoSimulasi/seaqistanam.svg" width="173px" height="206px" alt=""/>
      <v-collapse v-if="showChemistry">
        <!-- Additional content for Chemistry -->
        <p>Details about Chemistry simulation...</p>
      </v-collapse>
    </div>
  </div>
</template>

<script setup>
// Reactive variables for toggling show more functionality
import { ref } from 'vue';

const showBiology = ref(false);
const showPhysics = ref(false);
const showChemistry = ref(false);

// Toggle functions to show/hide content
const toggleBiology = () => showBiology.value = !showBiology.value;
const togglePhysics = () => showPhysics.value = !showPhysics.value;
const toggleChemistry = () => showChemistry.value = !showChemistry.value;
</script>

<style scoped>
.section-title {
  border-bottom: 2px solid #ccc; /* Add border under the title */
  padding-bottom: 10px;
  margin: 0; /* Remove margin to allow the line to extend fully */
  font-size: 24px;
  display: inline-block;
  width: 100%; /* Set width to 100% to extend the line */
}

.title-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
}

.show-more-btn {
  display: flex;
  align-items: center;
  color: #007bff; /* Optional: style for "Show More" button */
  padding: 0;
}

.show-more-btn v-icon {
  margin-left: 5px;
}
</style>
