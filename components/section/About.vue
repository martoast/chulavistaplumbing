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
              Don’t tackle plumbing issues on your own.
            </h2>

            <p class="subtitle-1">
              At chula vista plumbing, we offer fast turnaround and affordable rates. Even a relatively simple plumbing project can quickly take twists and turns you didn’t expect. Put your mind at ease, and let us take care of your plumbing needs. If you are working with other contractors, we can coordinate our efforts to ensure that your project is completed on time. Our plumbing services include:
            </p>
            <p class="mb-5">
              General plumbing needs, Drain cleaning, Tankless and traditional water heater installation, Pipe inspection and installation, Sewer inspection and related services. At Primo Plumbing, we build our schedule around your needs. We are available every day of the week, so call us for an estimate. We look forward to being your Chula Vista, CA, plumber.
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
    image: require("@/assets/plumbinghero.jpg")
  }),
  components: { SectionHeader }
};
</script>
