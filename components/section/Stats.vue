<template>
  <div>

    <section id="stats">

      <v-parallax
        :height="$vuetify.breakpoint.smAndDown ? 700 : 500"
        :src="this.hero"
      >

        <v-container fill-height>

          <v-row class="mx-auto">
            <v-col
              v-for="[value, title] of stats"
              :key="title"
              cols="12"
              md="3"
            >
              <div class="text-center">
                <div>
                  <v-icon
                    dark
                    x-large
                  >mdi-star</v-icon>
                </div>

                <div
                  class="headline font-weight-cold text-uppercase"
                  v-text="title"
                ></div>
              </div>
            </v-col>
          </v-row>
        </v-container>
      </v-parallax>
    </section>
  </div>
</template>
<script>
import SectionHeader from "~/components/section/SectionHeader.vue";
export default {
  components: { SectionHeader },
  data() {
    return {
      stats: [
        ["#1", "Same Day Appointments"],
        ["1000+", "Highly Trained Technicians"],
        ["100%", "Affordable Prices"],
        ["5 yrs", "Licensed, Bonded, and Insured Plumbers"]
      ],
      hero: require("@/assets/plumbinghero.jpg")
    };
  }
};
</script>
