<template>
  <div class="hello">
    <h1>Resume</h1>
    <Experience />
    <Skills />
  </div>
</template>

<script>
import Experience from "./Experience";
import Skills from "./Skills";

export default {
  components: {
    Experience,
    Skills
  }
};
</script>
