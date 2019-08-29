<template>
  <div>

    <v-card>
      <v-card-title class="subtitle primary--text font-weight-thin">References</v-card-title>
      <v-card
        v-for="reference in references"
        :key="reference.id"
        elevation="8"
      >
        <v-card-title>{{ reference.name }}</v-card-title>

        <v-card-text class="overline">

          {{reference.position}}
          <br>
          {{reference.company}}
          <br>
          {{reference.phone}}
          <br>
          {{reference.email}}
        </v-card-text>

      </v-card>
    </v-card>

  </div>
</template>

<script>
export default {
  data: () => ({
    references: [
      {
        name: "Ana Rivera",
        position: "Manager-Title Agent",
        company: "Central Florida Title Center LLC",
        phone: "407-696-3505",
        email: "ana@cftitle.com"
      },
      {
        name: "Salvatore Raitano",
        position: "Middle Office-Derivatives",
        company: "Bank of New York",
        phone: "407-493-4960",
        email: "salraitano@gmail.com"
      }
    ]
  })
}
</script>

<style lang="scss" scoped>
</style>