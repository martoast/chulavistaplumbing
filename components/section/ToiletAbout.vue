<template>
  <div>
    <section>
      <v-container>
        <div class="py-2" />
        <SectionHeader
          sub-header="Chula vista water Toilet repair/installation and plumbing services"
          header="chula vista plumbing"
        />
        <v-row>
          <v-col
            cols="12"
            md="6"
          >
            <h2
              :class="[$vuetify.breakpoint.mdAndUp ? 'display-1' : 'headline']"
              class="mb-4"
            >
              TOILET PLUMBING & REPAIRS: Leaks, Clogs & Installations
            </h2>

            <p class="subtitle-1">
              At The Plumber Inc., we’re dedicated to always being available. And we feel that it’s simply necessary in order to meet the demands of our customers. For emergencies, we’re available every hour of the day for seven days per week. This means that you never need to worry about leaks or clogs. If you’re in need of maintenance, repairs or want to install a new toilet, we’re also happy to help. With a wide range of both commercial and residential customers, we’ve got the experience and know-how to offer you the best possible results.
            </p>
            <p class="mb-5">
              Toilet problems are often unavoidable. But by being proactive, you can often avoid costly repairs. Contact us and we’ll help you diagnose and fix any problem you might be experience.
            </p>

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
          <v-col
            cols="12"
            md="5"
            offset-md="1"
          >
            <div class="hidden-md-and-down">
              <v-card flat>
                <v-img
                  :src="this.image"
                  height="500"
                  contain
                >
                </v-img>
              </v-card>

            </div>

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
    image: require("@/assets/toilet.jpg")
  }),
  components: { SectionHeader }
};
</script>
