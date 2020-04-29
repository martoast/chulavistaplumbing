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
              With many years of collective experience in dealing with even the most troublesome drain problems, we simply know how to fix pipes. No matter if we’re talking about pipe scale, buildups or just your average clogging, they’re all common causes for leaks and overflowing drains. And if not properly dealt with, they can lead to serious issues that in time will affect the entire building.
            </p>
            <p class="mb-5">
              We are fully equipped when it comes to cleaning drains, pipes and sewers. Due to a wide range of machines we have to ability to take care of everything ranging from even the smallest to the largest clog. This also means our efficiency is good enough to directly deal with most issues on location, within the shortest possible time frame. Our fully equipped vehicles can also deliver any needed extra equipment and material to accommodate all needs. We always make sure to use the right tools for the job, which might mean mechanical cleaning, jet flushing or whatever is needed to fix your problem.
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
