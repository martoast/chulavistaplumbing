<template>
  <div>
    <div>

      <v-footer
        dark
        height="auto"
        padless
      >

        <v-row class="ma-0">
          <v-col
            class="py-5 black white--text"
            cols="12"
            md="3"
          >

            <!-- <h3 class="headline mb-3">Boost Media Inc</h3> -->
            <ul class="body-1 pl-0">
              <li
                v-for="(c, i) in company"
                :key="i"
                class="mb-3"
              >
                <a
                  class="transition-swing"
                  v-text="c.title"
                  :href="c.link"
                />
              </li>
            </ul>
          </v-col>
          <v-col
            class="black white--text pa-5"
            cols="12"
            md="9"
          >
            <v-row class="hidden-sm-and-down">
              <v-col
                v-for="(category, i) in categories"
                :key="i"
                cols="12"
                md="6"
              >
                <v-btn
                  text
                  v-text="category.title"
                  :to="category.link"
                ></v-btn>
              </v-col>
            </v-row>
          </v-col>

          <v-col
            class="text-center black white--text pa-3"
            cols="12"
          >&copy; 2020 Chula Vista Plumbing — All Rights reserved.</v-col>
        </v-row>
      </v-footer>
    </div>
    <!-- <div>
      <v-footer
        dark
        padless
      >
        <v-card
          class="flex"
          flat
          tile
        >
          <v-card-title class="black">
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-4"
              dark
              icon
            >
              <v-icon size="24px">{{ icon }}</v-icon>
            </v-btn>
          </v-card-title>

        </v-card>
      </v-footer>
    </div> -->

  </div>
</template>

<script>
export default {
  components: {},
  data: () => ({
    categories: [
      {
        title: "Water Heater Installation or Replacement",
        link: "/services/waterheater"
      },
      {
        title: "Pressure Regulators & Shut Off Valves",
        link: "/services/waterlineleaks"
      },
      {
        title: "Leaking Faucets & Faucet Replacement",
        link: "/services/waterlineleaks"
      },
      {
        title: "Toilet Repairs",
        link: "/services/toiletrepairs"
      },
      {
        title: "High Pressure Drain Cleaning",
        link: "/services/draincleaning"
      },
      {
        title: "Sewer Line Replacement",
        link: "/services/sewer-repair"
      }
    ],
    company: [
      { title: "About", link: "/about/" },
      { title: "Services", link: "/services/" },

      { title: "Contact us", link: "/contact" }
    ],
    icons: [
      "mdi-facebook",
      "mdi-twitter",
      "mdi-google-plus",
      "mdi-linkedin",
      "mdi-instagram"
    ]
  })
};
</script>

<style lang="sass">
.v-application .v-footer
  ul
    list-style-type: none

    a
      color: white
      text-decoration: none

      &:hover
        color: grey
</style>
