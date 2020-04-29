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
              Jet Drain Cleaning for Clogged Mainlines in Phoenix
            </h2>

            <p class="subtitle-1">
              The main line is in many ways the most important drain. This means that clogged man lines can lead to serious issues if not quickly dealt with. But such clogs can be hard to find since it’s often not apparent exactly where the problem lies. We’ll identify and properly address the problem with the help of rooter machines, hydro jets or whatever is needed to unclog the main line.
            </p>
            <p class="mb-5">
              We have the needed equipment to deal with even the largest main line obstruction. By making sure to properly evaluate the problem at hand, we can apply the proper measures to effectively solve your problem. A big part of this is being able to actually access the main line. Our experience technicians have the right amount of know-how to deal with both older and modern mainlines.
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
    image: require("@/assets/draincleaning2.jpg")
  }),
  components: { SectionHeader }
};
</script>
