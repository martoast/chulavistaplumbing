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
                height="100%"
              >
              </v-img>
            </v-card>
          </v-col>
          <v-col
            cols="12"
            md="6"
          >
            <h2
              :class="[$vuetify.breakpoint.mdAndUp ? 'display-1' : 'headline']"
              class="mb-4"
            >
              Important Anode Rod Information
            </h2>

            <p class="subtitle-1">
              The anode rod is a vital part of every water heater. But unfortunately, it often becomes very corroded. This is unavoidable since the rod is actually supposed to attract the corrosive elements of the water. It’s basically a part of the heaters protection system, ensuring that the major components are spared from corrosion. By regularly replacing the anode rod, you can increase the lifespan of your water heater and make sure that it’s functioning properly for years to come. For people in and around Phoenix, The Plumber Inc., has become a trusted choice for anode rod replacements.
            </p>
            <p class="mb-5">
              By making sure to regularly maintain the anode rod, you can avoid having to buy a new water heater. This means huge savings. In many cases, this relatively simply fix can double or even triple the expected lifespan of a water heater. We have the experience to proper replace anode rods, and the knowledge to know when it’s time to do it. Contact The Plumber Inc., for a free consultation. We’ll make sure your water heater gives you the most bang for your buck.
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

        </v-row>
      </v-container>
    </section>
  </div>
</template>
<script>
import SectionHeader from "~/components/section/SectionHeader.vue";
export default {
  data: () => ({
    image: require("@/assets/waterheaterrods.jpg")
  }),
  components: { SectionHeader }
};
</script>
