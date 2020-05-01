<template>
  <div>

    <v-app-bar
      v-scroll="onScroll"
      color="indigo"
      :flat="!isScrolling"
      app
    >
      <VuetifyLogo />

      <v-spacer />
      <div class="hidden-md-and-up">

        <v-toolbar-items>
          <v-btn
            to="/contact"
            dark
            color="success"
            class="mr-12"
          >
            Contact Us
          </v-btn>
          <v-icon
            @click.stop="drawer = !drawer"
            dark
          >mdi-menu</v-icon>
        </v-toolbar-items>
      </div>
      <div class="hidden-sm-and-down">
        <v-menu offset-y>
          <template v-slot:activator="{ on }">

            <v-toolbar-items>
              <v-btn
                v-for="(item, i) in items"
                v-on="on"
                :key="i"
                :active-class="!isScrolling ? 'primary--text' : undefined"
                :to="item.to"
                text
                dark
              >
                <span v-text="item.text" />
              </v-btn>
            </v-toolbar-items>
          </template>
          <v-list light>
            <v-list-item
              v-for="(item, index) in Menuitems"
              :key="index"
            >
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item>
          </v-list>

        </v-menu>

      </div>
    </v-app-bar>
    <div>
      <v-navigation-drawer
        v-model="drawer"
        :right="right"
        temporary
        fixed
        src="https://cdn.vuetifyjs.com/images/backgrounds/bg-2.jpg"
        light
      >
        <v-list>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="title">
                Chula Vista Plumbing
              </v-list-item-title>
              <v-list-item-subtitle>
                We got you covered.
              </v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>

          <v-divider></v-divider>

          <v-list-item
            v-for="item in Menuitems"
            :key="item.title"
            link
            :to="item.to"
          >

            <v-list-item-content>
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item-content>

          </v-list-item>
        </v-list>
      </v-navigation-drawer>
    </div>
  </div>
</template>

<script>
// Utilities
import { mapMutations } from "vuex";
import VuetifyLogo from "~/components/VuetifyLogo.vue";

export default {
  components: {
    VuetifyLogo
  },
  data: () => ({
    isScrolling: false,

    clipped: false,
    drawer: false,
    fixed: false,
    miniVariant: false,
    right: true,
    rightDrawer: false,
    title: "Vuetify.js",
    Menuitems: [
      { title: "Home", icon: "mdi-home-city", to: "/" },
      {
        title: "Water Heater Services",
        icon: "dashboard",
        to: "/services/draincleaning/"
      },
      {
        title: "Repiping",
        icon: "dashboard",
        to: "/services/repiping"
      },
      {
        title: "Sewer Repair",
        icon: "dashboard",
        to: "/services/sewer-repair/"
      },
      {
        title: "Toilet Repair",
        icon: "dashboard",
        to: "/services/toiletrepairs/"
      },
      {
        title: "Water Line Leaks",
        icon: "dashboard",
        to: "/services/WaterLeaks/"
      },
      { title: "Contact Us", icon: "dashboard", to: "/contact" }
    ]
  }),
  computed: {
    items() {
      return [
        {
          to: "/",
          text: "Home"
        },
        {
          to: "/services/",
          text: "Services"
        },
        {
          to: "/about",
          text: "About"
        },
        {
          to: "/contact",
          text: "Contact"
        }
      ];
    }
  },

  methods: {
    ...mapMutations(["toggleDrawer"]),
    onScroll() {
      this.isScrolling =
        (window.pageYOffset || document.documentElement.scrollTop || 0) > 25;
    }
  }
};
</script>
