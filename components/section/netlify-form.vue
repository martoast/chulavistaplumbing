<template>
  <v-container
    fill-height
    id="contact-us"
  >
    <form
      name="contactus"
      action="/thanks"
      method="post"
      netlify
      netlify-honeypot="bot-field"
    >
      <input
        type="hidden"
        name="form-name"
        value="contactus"
      />
      <v-container fill-height>
        <v-card
          color="transparent"
          flat
        >
          <SectionHeader
            header="Contact Chula Vista plumbing today!"
            subHeader="Tell us what your issue is and we will send a team of experts to fix it!"
          />
          <v-row>
            <v-col cols="12">
              <div>
                <v-text-field
                  label="Name*"
                  for="name"
                  type="text"
                  name="name"
                  outlined
                  required
                  color="#404b87"
                />
              </div>
            </v-col>
            <v-col cols="12">
              <div>
                <v-text-field
                  label="Email*"
                  for="email"
                  type="email"
                  name="email"
                  required
                  outlined
                  color="#404b87"
                />
              </div>
            </v-col>

            <v-col cols="12">
              <div>
                <v-text-field
                  label="Phone #*"
                  for="phone"
                  name="phone"
                  required
                  outlined
                  color="#404b87"
                />
              </div>
            </v-col>
            <v-col cols="12">
              <v-select
                :items="['Water Heater', 'Drain Cleaning','Repiping','Sewer Services','Toilet Services','WaterLine Services' ]"
                label="What are you looking for*"
                for="looking4"
                name="lookining4"
                required
                outlined
              ></v-select>
            </v-col>

            <v-col cols="12">
              <div>
                <v-textarea
                  label="Your Message*"
                  for="message"
                  name="message"
                  required
                  outlined
                  color="#404b87"
                />
              </div>
            </v-col>
            <div>
              <v-container>
                <v-btn
                  type="submit"
                  value="Send message"
                  color="#404b87"
                  dark
                  block
                  x-large
                  outlined
                >Enviar</v-btn>
              </v-container>
            </div>
          </v-row>
        </v-card>
      </v-container>
    </form>
  </v-container>
</template>
<script>
import SectionHeader from "~/components/section/SectionHeader";
export default {
  components: { SectionHeader },
  data() {
    return {
      form: {
        name: "",
        email: "",
        message: ""
      }
    };
  },
  methods: {
    encode(data) {
      return Object.keys(data)
        .map(
          key => `${encodeURIComponent(key)}=${encodeURIComponent(data[key])}`
        )
        .join("&");
    },
    handleSubmit() {
      fetch("/", {
        method: "POST",
        headers: { "Content-Type": "application/x-www-form-urlencoded" },
        body: this.encode({ "form-name": "contact", ...this.form })
      })
        .then(() => alert("Success!"))
        .catch(error => alert(error));
    }
  }
};
</script>
