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
                  <v-theme-provider dark>
                    <div>
                      <v-avatar
                        color="primary"
                        size="88"
                      >
                        <v-icon
                          large
                          v-text="icon"
                        ></v-icon>
                      </v-avatar>
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
          icon: "mdi-account-group-outline",
          title: "Water Heater Installation/Replacement",
          text:
            "We provide full-service water heater repair and replacement. This includes both Tankless and Tank water heaters, so don't hesitate to contact us today."
        },
        {
          route: "/services/draincleaning",
          icon: "mdi-chart-line",
          title: "Pressure Regulators & Shut Off Valves",
          text:
            "Whether your challenge involves Pressure Regulators, shut off valves, or anything in between we can diagnose the problem and then make the repair."
        },
        {
          route: "/",
          icon: "mdi-cellphone-link",
          title: "Leaking Faucets & Faucet Replacement",
          text:
            "It's one of the most common repairs. But leaking faucets can be annoying and costly. Call today to get that leaky faucet fixed once and for all."
        },
        {
          route: "/services/toiletrepairs",
          icon: "mdi-account-group-outline",
          title: "Toilet Repairs",
          text:
            "Valve repairs are simple jobs in theory. But in reality they can be tricky and even difficult if you don't have the right tools. We can help."
        },
        {
          route: "/services/draincleaning",
          icon: "mdi-chart-line",
          title: "Drain Cleaning",
          text:
            "We take pride in keeping up with the latest technology when it comes to maximizing results. This includes all high pressure jetting jobs."
        },
        {
          route: "/services/sewer-repair/",
          icon: "mdi-cellphone-link",
          title: "Sewer Line Replacement",
          text:
            "If you want sewer line replacement or relining and clean out installation, give us a call. We will do the job right."
        }
      ]
    };
  }
};
</script>
