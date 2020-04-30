<template>
  <section
    id="contact"
    class="py-5"
  >
    <!-- <SectionHeader
      header="Work with Boost"
      sub-header="Contact Us"
    /> -->

    <v-container>
      <v-row>
        <v-col
          xs12
          md6
        >
          <Netlify />
        </v-col>

        <v-col
          cols="12"
          md="6"
        >
          <v-container
            fluid
            pa-0
          >
            <v-row>
              <v-col
                cols="12"
                md="6"
                class="pa-0"
              >
                <v-card-title>Mailing Address</v-card-title>
                <v-card-text>
                  <div>2365 palomira ct</div>
                  <div>Chula Vista, CA</div>
                  <div>United States</div>
                </v-card-text>
              </v-col>

              <v-col
                cols="12"
                md="6"
                class="pa-0"
              >
                <v-card-title>Contact Info</v-card-title>
                <v-card-text>
                  <div>+1 (619) 888-5248</div>
                  <div>
                    <a href="#">alexmartos96@gmail.com</a>
                  </div>

                </v-card-text>
              </v-col>

              <v-col cols="12">

                <iframe
                  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d53760.59455607247!2d-117.05954951625577!3d32.631833873670566!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x80d94e4565c3aacf%3A0x46ccb8734b8f2bd3!2sChula%20Vista%2C%20CA%2C%20USA!5e0!3m2!1sen!2smx!4v1588236915086!5m2!1sen!2smx"
                  width="100%"
                  height="400"
                  frameborder="0"
                  style="border:0"
                  allowfullscreen
                />
              </v-col>
            </v-row>
          </v-container>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
import SectionHeader from "~/components/section/SectionHeader.vue";
import Netlify from "~/components/section/netlify-form.vue";
export default {
  data() {
    return {
      select: null,
      items: [
        "Ecommerce",
        "Website",
        "SEO",
        "Marketing",
        "Everything digial!",
        "Idk, lets talk."
      ]
    };
  },

  components: {
    SectionHeader,
    Netlify
  }
};
</script>
