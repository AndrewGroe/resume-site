<template>
  <v-app>
    <v-card>
      <v-app-bar app>
        <v-toolbar-title>
          <span class="headline text-uppercase">Andrew Groe</span>
          <span class="headline primary--text"> | </span>
          <span class="subtitle font-weight-thin">Software Developer</span>
        </v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn
          color="primary"
          href="https://github.com/AndrewGroe"
          target="_blank"
        >
          <span>My Github</span>
          <v-icon right>mdi-github-circle</v-icon>
        </v-btn>
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
