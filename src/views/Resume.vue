<template>
  <div>
    <v-container>
      <v-row>
        <v-col
          cols="12"
          sm="12"
          md="4"
          lg="3"
        >
          <Bio />
        </v-col>
        <v-col
          cols="12"
          sm="12"
          md="8"
          lg="6"
        >
          <Experience />
        </v-col>

        <v-col
          cols="12"
          sm="12"
          md="4"
          lg="3"
        >
          <Skills />
        </v-col>

        <v-col>
          <Education />
        </v-col>
        <v-col>
          <References />
        </v-col>

      </v-row>
    </v-container>

  </div>
</template>

<script>
import Bio from "../components/Bio";
import Experience from "../components/Experience";
import Skills from "../components/Skills";
import References from "../components/References";
import Education from "../components/Education";

export default {
  components: {
    Bio,
    Experience,
    Skills,
    References,
    Education
  }
};
</script>
