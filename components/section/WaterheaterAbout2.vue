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
              Anode Rod, a major part of the water heater, is highly susceptible to corrosion. Unfortunately, this process of corrosion is inevitable in all water heaters as the rod attracts corrosive elements of water. However, in taking this damage upon itself, Anode Rod serves as the heater’s protection system by protecting other components of the system from corrosion. So, if you want to boost the lifespan of your water heater, you need to replace the anode rod regularly. This way, your heating system can continue performing its function efficiently for a long period of time. Chula Vista Plumbing offers anal rod replacement service at a very reasonable price to people of Pheonix and the surrounding areas.
            </p>
            <p class="mb-5">
              Don’t hesitate to replace the anode rods in your water heater in time as it can save you from spending more. You might end up needing to buy a new water heater for your hesitance to replace the rods. In taking the right decision of changing the rods occasionally, the lifespan of the water heater can be doubled and even tripled. Feel free to take free consultations from the professionals at Chula Vista Plumbing. We will make sure that your heater will be up and running for a number of years.
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
