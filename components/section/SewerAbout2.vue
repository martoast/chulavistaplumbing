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
                <v-list-item-title class="display-1">When should you consider to replace or repair the sewer line: </v-list-item-title>
                <v-list-item>Pipes are more than 50 years old</v-list-item>
                <v-list-item>Presence of persistent distinct smell</v-list-item>
                <v-list-item>The frequency of clogging and buildups is high</v-list-item>
                <v-list-item>The draining of water has slowed down drastically</v-list-item>

              </v-list>

            </div>
            <div class="pt-2">
              <p>However, the above points don’t cover all the issues that point out a sewer line problem. The good thing about the problem in the sewer line is that they need not be replaced and repairing them can solve the problem usually. Contact us to find out the severity of the issue. While we will try our best to repair the line but some lines are beyond repair and need replacement. In such cases, we can still help you by providing you sewer replacement service at an affordable price.
              </p>

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
