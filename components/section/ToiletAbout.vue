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
              TOILET PLUMBING & REPAIRS: Leaks, Clogs & Installations
            </h2>

            <p class="subtitle-1">
              While the toilet issues are unexpected, you should always try to act in advance to avoid unnecessary costs of repairs. Furthermore, repairing the issues in the toilet is an urgent matter. Keeping that in mind, we, at Chula Vista Plumbing, extend our services every day of the week and for all hours so that your issues are solved in time.
            </p>
            <p class="mb-5">
              If you are in need of repairing leaks or clogs in your toilet, you can contact us and we will get back to you swiftly. Also, you can count on us to repair or install a new toilet in your commercial and residential areas. Reach out to us and we assure you that your issue will be properly diagnosed and fixed for good.
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
    image: require("@/assets/toilet.jpg")
  }),
  components: { SectionHeader }
};
</script>
