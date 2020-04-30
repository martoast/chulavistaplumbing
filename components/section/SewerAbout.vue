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
              Sewer line repair and replacement in Chula Vista
            </h2>

            <p class="subtitle-1">
              Even though sewer lines are definitely built to last, nothing lasts for ever. Time takes its natural toll, and unexpected damage might also occur. Luckily, many problems can be fixed and with proper maintenance you won’t have to consider a replacement for years to come. But when replacement becomes a reality, we’ve got you covered. At The Plumber Inc., we can offer quality sewer line replacements in and around Phoenix.
            </p>
            <p class="mb-5">
              With many years of collective experience, we’re very aware of what makes a sewer line replacement successful. We’ll do everything we can in order to ensure that you’re satisfied with the results. Contact us today for a quote. We’re looking forward to hearing from you.
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
    image: require("@/assets/sewerrepair.jpg")
  }),
  components: { SectionHeader }
};
</script>
