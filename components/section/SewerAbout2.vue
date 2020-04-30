<template>
  <div>
    <section>
      <v-container>
        <div class="py-2" />
        <!-- <SectionHeader
          sub-header="Chula vista premium plumbing services"
          header="chula vista plumbing"
        /> -->
        <v-row>
          <v-col
            cols="12"
            md="5"
            offset-md="1"
          >
            <v-card flat>
              <v-img
                :src="this.image"
                height="400"
                contain
              >
              </v-img>
            </v-card>
          </v-col>
          <v-col
            cols="12"
            md="6"
          >
            <!-- <h2
              :class="[$vuetify.breakpoint.mdAndUp ? 'display-1' : 'headline']"
              class="mb-4"
            >
              Installation and repair of residential toilets
            </h2>

            <p class="subtitle-1">
              There are times when you simply want a new toilet, or when you feel that repairs are unavoidable. But dealing with these things on your own can be risky business. Not only will an improper job increase the risk of damage, but doing things on your own usually requires too much time and dedication. When contacting us, you’ll always get a great quote and you can be sure of the fact that we will respect your time. Contact The Plumber Inc., and let us make sure that your repair or installation becomes a great experience.
            </p>
            <p class="mb-5">
              Leaks are very common problems. But that doesn’t mean they’re any less of a hassle. Fortunately, they can often be fixed without having to replace the entire toilet. With access to a wide range of tools and components, we can take care of even the most pesky leaks. Thanks to many years of experience, our technicians can fix valves, gaskets, rings and all other things that are often associated with leaks.
            </p> -->
            <div class="headline">
              <v-list>
                <v-list-item-title class="display-1">Replacement or repairs might be a good idea when: </v-list-item-title>
                <v-list-item>Your existing pipes are pushing five decades old</v-list-item>
                <v-list-item>You are experiencing regular clogging and buildups</v-list-item>
                <v-list-item>You are noticing non-specific issues with your sink, toilet and such</v-list-item>
                <v-list-item>The water is not draining as quickly as it used to</v-list-item>
                <v-list-item>There is a distinct smell that doesn’t go away</v-list-item>
              </v-list>

            </div>
            <div class="pt-2">
              <p>These are only a few examples of things that might indicate a problem with your sewer line. But they don’t necessarily mean that you’re in need of a replacement. More often than not, repairs are enough. By contacting us, we can arrange a proper inspection to see what needs to be done. Hopefully, it will only be a minor issue. But if you’re in need of a new sewer line, we can absolutely arrange one. We can offer very competitive prices ensuring that you stay on budget.</p>

            </div>

            <v-btn
              outlined
              color="primary"
              class="px-5"
              large
              to="/contact"
            >
              Contact Us
            </v-btn>
          </v-col>

        </v-row>
      </v-container>
    </section>
  </div>
</template>
<script>
import SectionHeader from "~/components/section/SectionHeader.vue";
export default {
  data: () => ({
    image: require("@/assets/sewer.jpg")
  }),
  components: { SectionHeader }
};
</script>
