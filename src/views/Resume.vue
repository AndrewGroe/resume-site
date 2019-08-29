<template>
  <div>
    <v-container>
      <v-row>
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
          md="6"
          lg="2"
        >
          <Skills />
        </v-col>

        <v-col
          cols="12"
          sm="12"
          md="6"
          lg="3"
        >
          <Education />
        </v-col>

        <v-col
          cols="12"
          sm="12"
          md="6"
          lg="3"
        >
          <References />
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
