<template>
  <div>
    <section>
      <v-container>
        <div class="py-2" />
        <SectionHeader
          sub-header="Chula vista premium plumbing services"
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
              Let professionals handle your plumbing issues.
            </h2>

            <p class="subtitle-1">
              For many years now, we, at Chula Vista Plumbing, have been serving our community in the Phoenix Metro area with excellent plumbing services. Our representatives are the best professionals, with a high level of training and expertise, that you can find in the region. So, if you are concerned with your plumbing issues at hand, seek no further. Here, at Chula Vista Plumbing, you will find solutions to all of your plumbing needs.
            </p>
            <p class="mb-5">
              We extend our services to both commercial and residential plumbing needs. Some of the services that we provide, but not limited to, are Drain Cleaning, Pipe Inspection and Installation to Sewer Inspection, Tankless and Traditional Water Heater Installation and all the general plumbing needs. Our services are available every day of the week. Also, just let us know your schedule and we will facilitate the service accordingly. We look forward to becoming a one-stop solution to all your plumbing needs at Chula Vista, CA.
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
            <v-card class="hidden-sm-and-down">
              <v-img
                :src="this.image"
                height="500"
              >
              </v-img>
            </v-card>
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
    image: require("@/assets/plumbing.png")
  }),
  components: { SectionHeader }
};
</script>
