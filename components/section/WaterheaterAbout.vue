<template>
  <div>
    <section>
      <v-container>
        <div class="py-2" />
        <SectionHeader
          sub-header="Chula vista water heater installation and plumbing services"
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
              Chula Vista Water Heater Plumbers
            </h2>

            <p class="subtitle-1">
              A broken water heater poses a major concern for people which needs to be attended to immediately. Here, at Chula Vista Plumbing, you will find plumbing experts ready to be at your service anytime to rid you of your issues. Our professionals are well equipped to fix even the oldest of water heater versions to the most latest ones. In cases that the old water heater can be repaired, our professionals will put their utmost effort to increase the working period of the heater. However, if the heater cannot be repaired, you can trust us to deliver you the latest, efficient and reliable water heater at a reasonable price.
            </p>
            <p class="mb-5">
              One of the reasons for our ability to deliver positive customer experience and trust is because we are clear in discussing all the costs involved in the process. Before beginning the work, we provide you with a price estimation or the final amount and we make sure that we will work under the discussed price. We assure you that there will be no unexpected costs or hidden fees during or after work.
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
    image: require("@/assets/waterheater.png")
  }),
  components: { SectionHeader }
};
</script>
