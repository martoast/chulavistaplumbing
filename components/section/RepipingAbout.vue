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
              Pipes tend to corrode over the years due to which they need to be repaired or replaced. Not taking care of the pipes on time can result in huge costs to be incurred in the future. Not only that, but you will also have to go through the trouble of all the leaking and spreading of the water, gas or sewage that runs through the pipes, in your property. Letting our plumbers at Chula Vista Plumbing to repipe the worn-out pipes will ensure the safety of the gas, water and sewage pipes while they are transported through the walls and under the floors to the designated place.
            </p>
            <p class="mb-5">
              Many people fail to see the clear advantages of repiping. Also, what they fail to realize is that insurance might not cover the damage due to leaking or damaged pipes. You might end up with a heavy bill to pay in replacing your old pipes in addition to the amending the damage done by the old pipes to your property. So, take the professional help of Chula Vista plumbers in repiping your home or commercial business.
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
