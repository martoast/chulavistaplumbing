<template>
  <div>
    <section>
      <v-container>
        <div class="py-2" />
        <SectionHeader
          sub-header="Chula vista water heater installation and plumbing services"
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
              Chula Vista Water Heater Plumbers
            </h2>

            <p class="subtitle-1">
              A broken water heater can be a serious problem. And it’s often also an urgent matter. At The Plumber Inc., we are always available to instantly fix your heater. Our experience ranges from most of the major current brands to older no longer supported heaters. In most cases, we’ll be able to extend the life of even the oldest water heater. But if a repair is not possible, we’ll always make sure to offer you the best possible price for new installations of reliable models.
            </p>
            <p class="mb-5">
              An important part of our business model is to always provide you with an offer up front. This means that we’ll offer you a free quick consultation and provide you with either a price estimate or a final price that we actually stick to. This means that you’ll never have to worry about unexpected costs or become the victim of unreliable pricing models. By avoiding hidden fees, we have earned the trust of many customers in and around Phoenix. We’re looking forward to hearing from you.
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
    image: require("@/assets/waterheater.png")
  }),
  components: { SectionHeader }
};
</script>
