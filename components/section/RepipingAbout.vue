<template>
  <div>
    <section>
      <v-container>
        <div class="py-2" />
        <SectionHeader
          sub-header="Chula vista Re-Piping Plumbing Service"
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
              Re-piping services in Chula Vista
            </h2>

            <p class="subtitle-1">
              Over the years pipes can degrade and corrode and this can cost you thousands of dollars should they fail or leak. New pipes on your property can mean that your water, gas, and sewage is transported through your walls and under your floors safely and as designed. Letting your pipes go un-repaired or un-replaced can mean having all of that leaking and spreading throughout your property. Our Chula Vista Repiping service is the best in the area.
            </p>
            <p class="mb-5">
              It may seem obvious what the benefits of repiping your home or commercial business but what many don't understand is the damaged caused by leaking or damaged pipes are many times not covered by insurance. Old pipes failing fall under both water seepage and wear and tear and many homeowners are stuck with an unmanageable bill. Take control and repipe your property before it becomes an issue.
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
