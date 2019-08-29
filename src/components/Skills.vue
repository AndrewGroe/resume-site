<template>
  <div>
    <v-card class="pb-2">
      <v-card-title class="subtitle primary--text font-weight-thin">Skills</v-card-title>
      <v-card
        v-for="skill in this.skills"
        :key="skill.id"
        class="pa-2 mx-2 my-1"
        elevation="8"
      >
        <span>{{ skill.name }}</span>
        <v-rating
          dense
          class="text-center"
          :value="skill.proficiency"
          :empty-icon="skill.icon"
          :full-icon="skill.icon"
          color="primary"
          background-color="grey"
        ></v-rating>
      </v-card>
    </v-card>

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
      },
      {
        name: "Android",
        proficiency: 3,
        icon: "mdi-android"
      }
    ]
  })
};
</script>
