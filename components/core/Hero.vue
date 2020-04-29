<template>
  <v-img
    height="100vh"
    :src="this.hero"
    class="white--text"
    gradient="to top, rgba(13, 3, 29, .85), rgba(25.5, 41.2, 88.2, .85)"
  >
    <v-container fill-height>
      <v-row
        align="center"
        justify="center"
        class="pt-5 px-3"
      >
        <v-sheet
          color="transparent"
          dark
          max-width="500"
        >
          <h1 class='mb-4 display-2'>
            Chula Vista Plumbing
          </h1>

          <p class="title font-weight-light">
            <strong>Premier San Diego Plumber Serving All San Diego County</strong>
          </p>

          <div class="py-4" />

          <v-row
            class="ma-0"
            justify="center"
            justify-md="start"
          >
            <v-btn
              class="mr-md-3 my-2"
              color="white"
              large
              min-width="175"
              outlined
              rounded
              to="/about/"
            >
              Learn More
            </v-btn>

            <v-btn
              class="my-2"
              color="white"
              outlined
              large
              min-width="175"
              rounded
              href="tel: +1 (619) 888-5258"
            >
              <v-icon class="pa-2">mdi-phone-outgoing</v-icon>
              CALL NOW
            </v-btn>
          </v-row>
        </v-sheet>
      </v-row>
    </v-container>
  </v-img>
</template>

<script>
export default {
  data: () => ({
    hero: require("@/assets/plumbinghero.jpg")
  }),
  computed: {
    namespace() {
      return this.$route.name;
    }
  }
};
</script>
