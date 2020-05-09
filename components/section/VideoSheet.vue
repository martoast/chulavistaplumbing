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
                  With over two decades of experience serving Chula Vista, California and the adjacent areas, Chula Vista Plumbing has solutions to all of your plumbing necessities, whether it is just minor tweaks or major renovations. We keep ourselves updated with the latest technology and equipment, which is one of the reasons for our customers to be highly satisfied with us. Contact us for your needs and our plumbing experts will get to work in no time.
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
