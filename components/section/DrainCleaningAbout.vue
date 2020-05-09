<template>
  <div>
    <section>
      <v-container>
        <div class="py-2" />
        <SectionHeader
          sub-header="Chula vista drain services"
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
              Professional drain services
            </h2>

            <p class="subtitle-1">
              If the issues in the drain are not dealt with in time, they can cause major problems in the future which can affect the whole residential or commercial area. Whether it is pipe scale, buildups or minor clogging, they can lead to leaks and overflowing drains. These issues can compound with time to create big troubles. Contact our plumbers at Chula Vista who boast years of experience in handling drain issues.
            </p>
            <p class="mb-5">
              Furthermore, the availability of all the necessary equipment to clean pipes, sewers and drains ensures that the clogs of every scale, whether very small or large, are easily removed by our plumbers. Be it mechanical cleaning, jet flushing or any other necessary means, our plumbers make use of the best resource at hand to deal with the issue. In doing so, high efficiency is maintained and the task is completed in a short period of time.
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
    image: require("@/assets/dranecleaning.jpg")
  }),
  components: { SectionHeader }
};
</script>
