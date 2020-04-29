<template>
  <div>
    <v-layout
      column
      justify-center
      align-center
    >
      <v-flex
        xs12
        sm8
        md6
      >
        <About />
        <Stats />
        <DemoContact />
        <Services />
        <VideoSheet />

      </v-flex>

    </v-layout>
    <Contact />

  </div>

</template>

<script>
import VuetifyLogo from "~/components/VuetifyLogo.vue";
import Services from "~/components/section/Services.vue";
import VideoSheet from "~/components/section/VideoSheet.vue";
import About from "~/components/section/About.vue";
import Contact from "~/components/section/Contact.vue";
import Stats from "~/components/section/Stats.vue";
import DemoContact from "~/components/section/DemoContact.vue";

export default {
  components: {
    Services,
    VuetifyLogo,
    VideoSheet,
    About,
    Contact,
    Stats,
    DemoContact
  }
};
</script>
