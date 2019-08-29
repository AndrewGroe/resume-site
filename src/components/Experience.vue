<template>
  <div>

    <v-card class="pa-2">

      <v-card-title class="subtitle primary--text font-weight-thin">Work Experience</v-card-title>
      <v-card
        v-for="job in jobs"
        :key="job.id"
        class="pa-2 ma-2 pb-4"
        elevation="8"
      >
        <v-card-title>{{job.position}}</v-card-title>
        <v-card-text class="overline">

          {{job.company}}
          <br>
          {{job.dates}}
        </v-card-text>

        <ul>
          <li
            v-for="responsibility in job.responsibilities"
            :key="responsibility.key"
          >
            {{responsibility}}
          </li>
        </ul>
        <v-card-action>
          <v-btn
            color="primary"
            small
            v-if="job.links"
            :href="job.links.url"
          >{{job.links.name}}

            <v-icon
              small
              right
            >mdi-android</v-icon>

          </v-btn>
        </v-card-action>
      </v-card>

    </v-card>

  </div>
</template>

<script>
export default {
  data: () => ({
    jobs: [
      {
        company: "Central Florida Title Center",
        position: "IT / Development",
        dates: "2012-Present",
        responsibilities: [
          "Converting paper records to pdf format",
          "Consulting security measures as well as hardware and software upgrades",
          "Maintaining hardware and software both remote and onsite",
          "Creating and maintaining company website (cftitle.com)",
          "Creating and maintaining native mobile apps Android(Java) & iOS(Swift)"
        ],
        links: {
          name: "Android App",
          url: "https://tinyurl.com/cftcplaystore"
        }
      },
      {
        company: "Personal Projects",
        position: "Web & Mobile Development",
        dates: "2012-present",
        responsibilities: [
          "Comfortable with modern JavaScript (ES6+)",
          "Proficiency with various frontend frameworks",
          "Android development with Java and Kotlin",
          "Familiarity with common software architectures (MVVM, MVP, MVC)",
          "Experience with common Android 3rd party libraries (Retrofit, Glide, Room, etc.)",
          "Understanding of advanced Android topics like RxJava, Coroutines & Extension Functions, Dependency Injection, Data Binding and more",
          "Experience publishing to both Google Play Store and App Store"
        ]
      }
    ]
  })
};
</script>
