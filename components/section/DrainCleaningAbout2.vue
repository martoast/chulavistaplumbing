<template>
  <div>
    <section>
      <v-container>
        <div class="py-2" />

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
              The problems of clogs are not always easy to locate for people. As the main line is the most important drain line, issues of clogging in the main line can create major issues if they are not attended to at the right time. Our plumbing experts at Chula Vista Plumbing have access to equipment such as rooter machines and hydro jets, among other machines, to help them diagnose and solve the issue of clogging in the main line.
            </p>
            <p class="mb-5">
              What the Chula Vista plumbers do is evaluate the ongoing issue before deciding on a solution. Depending upon the evaluation, they devise the best possible way to deal with the issue, using the best possible equipment out of the range of equipment available to the plumbers. Whether an old or a new version of the main line, our technicians are well versed to deal with them.
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
