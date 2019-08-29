<template>
  <div>

    <v-card>
      <v-card-title class="subtitle primary--text font-weight-thin">Education</v-card-title>
      <v-card
        v-for="school in schools"
        :key="school.id"
        elevation="8"
      >
        <v-card-title>{{ school.diploma }}</v-card-title>

        <v-card-text class="overline">
          <span
            class="font-weight-thin body-1"
            v-if="school.focus"
          >
            {{school.focus}}
          </span>
          <br>
          {{school.name}}
          <br>
          {{school.location}}
          <br>
          {{school.date}}
        </v-card-text>

      </v-card>
    </v-card>
  </div>
</template>

<script>
export default {
  data: () => ({
    schools: [
      {
        name: "Valencia College",
        location: "Orlando, FL",
        date: "2018",
        diploma: "Associate's Degree",
        focus: "Computer Science",
        detail: "Completed various software engineering courses including C, Java and Android"
      },
      {
        name: "Bishop Moore Catholic High School",
        location: "Orlando, FL",
        date: "2012",
        diploma: "High School Diploma",
        focus: null,
        detail: "Recognized in the Florida Catholic newspaper for initiative and development skill after creating Android app for school without guidance"
      }
    ]
  })
}
</script>

<style lang="scss" scoped>
</style>