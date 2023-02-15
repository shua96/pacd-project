<template>
  <v-navigation-drawer v-model="drawer" :rail="rail" permanent @click="rail = false" app fixed clipped color="#4D68AF"
    light>
    <v-list-item prepend-avatar="src/assets/logo.png" title="TESDA-PACD" nav style="color: white;">
      <template v-slot:append>
        <v-btn variant="text" icon="mdi-chevron-left" @click.stop="rail = !rail"></v-btn>
      </template>
    </v-list-item>

    <v-divider></v-divider>

    <v-list density="compact" nav style="color: white;">
      <v-list-item prepend-icon="mdi-view-dashboard" title="DASHBOARD" value="dashboard"
        style="color: white;"></v-list-item>
      <v-list-item prepend-icon="mdi-frequently-asked-questions" title="FAQ LIST" value="faq"
        style="color: white;"></v-list-item>
      <v-list-item prepend-icon="mdi-database" title="CLIENT DATA" value="database" style="color: white;"></v-list-item>
      <v-list-item prepend-icon="mdi-poll" title="SUMMARY REPORT" value="report" style="color: white;"></v-list-item>
    </v-list>
  </v-navigation-drawer>
  <v-main style="height: 100vh"></v-main>
</template>

<script>
export default {
  data() {
    return {
      drawer: true,
      items: [
        { title: 'Home', icon: 'mdi-view-dashboard' },
        { title: 'FAQ LIST', icon: 'mdi-frequently-asked-questionst' },
        { title: 'CLIENT DATA', icon: 'mdi-database' },
        { title: 'SUMMARY REPORT', icon: 'mdi-poll' },
      ],
      rail: true,
    }
  },
}
</script>
