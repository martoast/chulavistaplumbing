<template>
  <div>
    <section
      id="features"
      class="grey lighten-3"
    >
      <v-container class="text-center">
        <SectionHeader
          header="Chula vista plumbing"
          sub-header="The Plumber Chula Vista Trusts Most"
        />

        <div>
          <v-item-group>
            <v-row>
              <v-col
                v-for="({ route,icon, title, text }, i) in features"
                :key="i"
                cols="12"
                md="4"
              >
                <v-card
                  class="py-12 px-4"
                  color="grey lighten-5"
                  flat
                  :to="route"
                >
                  <v-theme-provider light>
                    <div>

                      <v-icon
                        large
                        v-text="icon"
                      ></v-icon>

                    </div>
                  </v-theme-provider>

                  <v-card-title
                    class="justify-center font-weight-black text-uppercase"
                    v-text="title"
                  ></v-card-title>

                  <v-card-text
                    class="subtitle-1"
                    v-text="text"
                  > </v-card-text>
                </v-card>
              </v-col>
            </v-row>

          </v-item-group>
        </div>

      </v-container>

      <div class="py-12"></div>
    </section>
  </div>
</template>
<script>
import SectionHeader from "~/components/section/SectionHeader.vue";
export default {
  components: {
    SectionHeader
  },
  data() {
    return {
      features: [
        {
          route: "/services/waterheater/",
          icon: "mdi-checkbox-marked-circle-outline",
          title: "Water Heater Installation/Replacement",
          text:
            "Our water heater installation and replacement service include both tank and tankless water heaters. Feel free to contact us anytime and we will get back to you soon."
        },
        {
          route: "/services/waterlineleaks",
          icon: "mdi-checkbox-marked-circle-outline",
          title: "Water Line Leak Repairs",
          text:
            "Be it Shut Off Valves, Pressure Regulators, or any other similar problems, leave it to our plumbing experts to identify and solve the issue."
        },
        {
          route: "/services/repiping",
          icon: "mdi-checkbox-marked-circle-outline",
          title: "Leaking Faucets & Faucet Replacement",
          text:
            "As simple as it may seem, faucets can pose issues to every household. Get your faucet fixed or replaced quickly to save you from frustration."
        },
        {
          route: "/services/toiletrepairs",
          icon: "mdi-checkbox-marked-circle-outline",
          title: "Toilet Repairs",
          text:
            "While valve repairs might seem simple, without the necessary equipment you might not be able to do it yourself. In such a case, we are a call away from repairing them."
        },
        {
          route: "/services/draincleaning",
          icon: "mdi-checkbox-marked-circle-outline",
          title: "Drain Cleaning",
          text:
            "We handle all high pressure jetting jobs with modern technology, which increases the efficiency of work. "
        },
        {
          route: "/services/sewer-repair/",
          icon: "mdi-checkbox-marked-circle-outline",
          title: "Sewer Line Replacement",
          text:
            "Whether for sewer line replacement or sewer relining, our professionals are ready to help with your needs."
        }
      ]
    };
  }
};
</script>
