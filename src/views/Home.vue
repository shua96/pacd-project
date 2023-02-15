<template>
  <v-container>
    <v-row>
      <v-col cols="2">
        <NavBar />
      </v-col>
      <v-col cols="10">
        <v-layout row wrap justify-center>
          <!-- class="bg-purple-darken-2 text-center" -->
          <v-flex class="ma-0 pb-12">
            <h1>DASHBOARD</h1>
          </v-flex>
        </v-layout>
        <v-card class="mb-10 pa-3">
          <BarGraph />
        </v-card>
        <v-row justify="center">
          <v-col cols="6" class="pt-12">
            <v-card class="pa-3">
              <GenderPieGraph />
            </v-card>
          </v-col>
          <v-col cols="6" class="pt-12">
            <v-card class="pa-3">
              <AgePieGraph />
            </v-card>
          </v-col>
        </v-row>
        <v-row justify="center">
          <v-col cols="6" class="pt-12">
            <v-card class="pa-3">
              <ReasonForVisitPieGraph />
            </v-card>
          </v-col>
          <v-col cols="6" class="pt-12">
            <v-card class="pa-3">
              <ActionProvidedPieGraph />
            </v-card>
          </v-col>
        </v-row>

      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
import BarGraph from '@/components/BarGraph.vue';
import NavBar from '@/components/NavBar.vue';
import GenderPieGraph from '@/components/GenderPieGraph.vue';
import AgePieGraph from '@/components/AgePieGraph.vue';
import ReasonForVisitPieGraph from '@/components/ReasonForVisitPieGraph.vue';
import ActionProvidedPieGraph from '@/components/ActionProvidedPieGraph.vue';

</script>
