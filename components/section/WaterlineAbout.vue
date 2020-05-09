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
              Minor issues can build up over the years in your water line which will compound to create a major problem in the future, which includes blockage in water flow, leaking, flooding or mold development. So as to avoid such problems from occurring, necessary attention needs to be paid from time to time to keep your water line clean and free of any hindrances. Repairing the water line will not only save you from future troubles but will also rid you of the unnecessary costly repairs that you might have to incur when the situation worsens. Let our experts at Chula Vista Plumbing attend any services related to the maintenance of your water line.
            </p>
            <p class="mb-5">
              While many of the issues might be created by us along with the time that disrupts the flow of water in our water line, some of the unforeseen events include tree roots piercing the pipe or the cracking of the water line due to the shifting of the ground beneath the building. Or it might just be that the water line might be in need of replacement after years of use. Whatever the case, our team, at Chula Vista Plumbing, is always ready to fix the issue.

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
