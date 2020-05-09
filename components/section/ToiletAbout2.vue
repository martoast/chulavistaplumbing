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
                height="400"
                contain
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
              Installation and repair of residential toilets
            </h2>

            <p class="subtitle-1">
              While one might be tempted to repair the toilets on their own but it might not always be a good idea. You will need to spend a lot of time repairing the problem. Also, not having the right technique and equipment can lead to further damage. Or, you might simply want to replace your toilet with a new one. Whether to repair or replace your toilet, you can rely on the quality and affordable services provided by Chula Vista plumbers. Let us know your schedule and we will be there at your service at the designated time.
            </p>
            <p class="mb-5">
              While leaks are a minor issue in your toilets, they can be quite frustrating if they occur frequently. However, you will not need to replace your toilet mostly as leaks can be easily managed. With all the necessary equipment available to our Chula Vista plumbers, we can easily fix issues such as gaskets, rings, valves or any other issues that lead to the leakage.
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
    image: require("@/assets/toiletservice.jpg")
  }),
  components: { SectionHeader }
};
</script>
