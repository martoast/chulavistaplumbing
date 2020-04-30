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
              Chula Vista Water Line Leak Repairs & Services
            </h2>

            <p class="subtitle-1">
              Keeping your water line clean and free of obstruction is vital to preventing issues with water flow, flooding, leaking, and mold development. The water line provides water throughout your home or business. Water line leak repairs can be expensive so it can be essential to trust the maintenance of them to an accomplished Phoenix plumber. Our team of Phoenix leak repair experts at The Plumber Inc. we can provide you with dedicated water line services that can help avoid costly repairs in the future.
            </p>
            <p class="mb-5">
              Most people experience major problems with their water lines after small problems have compounded over time. Many people need repairs when tree roots end up piercing the pipe and preventing the flow of water through the pipe. Over time, the ground beneath your building can shift and create cracks in the water line. It might also be that the pipes supporting the water line are aged and not as effective as they used to be.
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
