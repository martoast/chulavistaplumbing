<template>
  <v-app dark>

    <AppBar />
    <Hero />

    <v-content>
      <nuxt />

    </v-content>

    <!-- <Testimonials /> -->

    <!-- <DemoContact /> -->

    <Footer />
  </v-app>
</template>

<script>
import AppBar from "~/components/core/AppBar.vue";
import Hero from "~/components/core/Hero.vue";

export default {
  components: {
    AppBar,
    Hero,

    Footer: () => import("~/components/core/Footer")
  },
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: "mdi-apps",
          title: "Welcome",
          to: "/"
        },
        {
          icon: "mdi-chart-bubble",
          title: "Inspire",
          to: "/inspire"
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Vuetify.js"
    };
  }
};
</script>
