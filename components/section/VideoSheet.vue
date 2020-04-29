<template>
  <div>
    <section class="grey lighten-3">
      <v-container>

        <SectionHeader
          sub-header="Why Chula vista plumbing?"
          header="Mastering Organic Growth"
        />
        <v-row
          align="center"
          justify="space-between"
        >
          <v-col
            cols="12"
            md="5"
            offset-xl="1"
          >

            <div class="ma-12">
              <v-row justify="center">
                <h2 class="mb-4 headline">
                  It all comes down to experience. <br />
                </h2>

                <p class="subtitle-1">
                  Primo Plumbing has been servicing Chula Vista, California and the surrounding areas for over two decades. We are available for all your plumbing needs.For more than 30 years, we have been offering exceptional customer service and staying current with the latest technology. Whether you just want to make minor updates, or you are planning extensive renovations, our plumbing contractors are ready to get to work.
                </p>

                <v-btn
                  outlined
                  color="#BF9B2A"
                  class="px-5"
                  x-large
                  to="/contact"
                >
                  Contact us
                </v-btn>

              </v-row>

            </div>

          </v-col>

          <v-col
            cols="12"
            md="5"
          >

            <div align="center">
              <v-container>

                <iframe
                  style="top:55px; left:0; bottom:0; right:0; height: 400px; border:none; margin:0; padding:0; z-index:999999;"
                  src="https://player.vimeo.com/video/404896466"
                  frameborder="0"
                  allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
                  allowfullscreen
                  width="100%"
                ></iframe>

              </v-container>

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
  components: { SectionHeader },
  data() {
    return {};
  }
};
</script>
