<template>
  <div>
    <v-flex xs12 md4>
      <v-card>
        <v-card-title>Experience</v-card-title>
        <v-list-item v-for="job in jobs" :key="job.id"></v-list-item>
      </v-card>
    </v-flex>
  </div>
</template>

<script>
export default {
  data: () => ({
    skills: [
      {
        name: "HTML",
        proficiency: 4,
        icon: "mdi-language-html5"
      },
      {
        name: "CSS",
        proficiency: 3,
        icon: "mdi-language-css3"
      },
      {
        name: "JavaScript",
        proficiency: 4,
        icon: "mdi-language-javascript"
      },
      {
        name: "Vue.js",
        proficiency: 3,
        icon: "mdi-vuejs"
      },
      {
        name: "Node.js",
        proficiency: 2,
        icon: "mdi-nodejs"
      },
      {
        name: "Java",
        proficiency: 3,
        icon: "mdi-language-java"
      }
    ]
  })
};
</script>
<style lang="scss" scoped>
</style>