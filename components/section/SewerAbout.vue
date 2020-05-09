<template>
  <div>
    <section>
      <v-container>
        <div class="py-2" />
        <SectionHeader
          sub-header="Chula vista water Toilet repair/installation and plumbing services"
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
              Sewer line repair and replacement in Chula Vista
            </h2>

            <p class="subtitle-1">
              While sewer lines might be known for their durability, they come with an expiration date too. So, they will need to be dealt with before any problems escalate from their damage due to time or by accident. Sewer lines won’t need a replacement for years but in case they do, you can count on our technicians at Chula Vista Plumbing to do the job for you in Phoenix and surrounding places.
            </p>
            <p class="mb-5">
              Years of experience in this field makes us a proper choice to make in replacing your sewer line.
              Don’t hesitate to contact us for any consultations for a price quote. We will make sure that you will be satisfied with our services.
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
