<template>
  <v-app>
    <v-card>
      <v-app-bar app>
        <v-spacer></v-spacer>
        
      </v-app-bar>
    </v-card>

    <v-content>
      <router-view />
    </v-content>
  </v-app>
</template>

<script>

export default {
  name: 'App',
  data: () => ({
    //
  }),
};
</script>
