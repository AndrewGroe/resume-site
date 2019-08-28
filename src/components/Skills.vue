<template>
  <div>
    <v-flex class="text-center" xs12 md2>
      <v-card>
        <v-card-title>Skills</v-card-title>
        <div v-for="skill in this.skills" :key="skill.id">
          {{ skill.name }}
          <v-rating
            dense
            :value="skill.proficiency"
            :empty-icon="skill.icon"
            :full-icon="skill.icon"
            color="primary"
            background-color="grey"
          ></v-rating>
        </div>
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