<template>
  <div class="about">
    <h1>saoco papi saoco - rosalia - ({{ likes }}) me gusta</h1>
    <v-btn
      prepend-icon="mdi-thumb-up"
      color="primary"
      @click="likes++"
      >
      Me gusta 
    </v-btn>
    <v-icon icon="mdi-home" color="black"></v-icon>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const likes = ref(0)
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
