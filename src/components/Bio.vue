<template>
  <v-container>
    <v-card>
      <v-col
        align-self="start"
        class="pa-0"
        cols="12"
      >
        <v-avatar
          class="profile"
          color="grey"
          size="164"
          tile
        >
          <v-img src="https://www.upwork.com/profile-portraits/c1sd_heZR2jnDg10GAvYHux_fJJrFpMhS2vApg1a0qMCEn3PXEC7jDj6zg1fs31rK-"></v-img>
        </v-avatar>
      </v-col>

      <v-card-title>Andrew Groe</v-card-title>
      <v-card-text>
        <span>{{email}}</span>
        <br>
        <span>{{location}}</span>
      </v-card-text>

      <v-card-text>Motivated and determined developer with fullstack web and native mobile development experience.
        Eager to join an agile team and contribute to the SDLC.
      </v-card-text>

      <v-card-actions>
        <div class="flex-grow-1"></div>
        <v-btn
          to="/about"
          color="primary"
        >More About Me</v-btn>
      </v-card-actions>
    </v-card>

  </v-container>
</template>

<script>
export default {
  data: () => ({
    name: "Andrew Groe",
    email: "andrewgroe.dev@gmail.com",
    location: "Orlando, FL"
  })
}
</script>

<style>
</style>
