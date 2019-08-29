<template>
  <div>
    <v-container>
      <v-row>

        <v-col cols="6">
          <Experience />
        </v-col>

        <v-col cols="3">
          <Skills />
        </v-col>

        <v-col cols="3">
          <v-col cols="12">
            <Education />
          </v-col>
          <v-col cols="12">
            <References />
          </v-col>
        </v-col>
      </v-row>
    </v-container>

  </div>
</template>

<script>
import Experience from "../components/Experience";
import Skills from "../components/Skills";
import References from "../components/References";
import Education from "../components/Education";

export default {
  components: {
    Experience,
    Skills,
    References,
    Education
  }
};
</script>
