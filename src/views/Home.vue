<template>
  <v-container>
    <v-row>
      <v-col cols="2">
        <NavBar />
      </v-col>
      <v-col cols="10">
        <ChartComponent />
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
import ChartComponent from '@/components/ChartComponent.vue'
import NavBar from '@/components/NavBar.vue';
</script>
