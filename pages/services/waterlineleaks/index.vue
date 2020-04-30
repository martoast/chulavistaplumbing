<template>
  <div>

    <About />
    <About2 />
    <Services />
    <Contact />

  </div>
</template>
<script>
import About from "~/components/section/WaterlineAbout.vue";
import About2 from "~/components/section/WaterlineAbout2.vue";
import Services from "~/components/section/Services.vue";
import Contact from "~/components/section/Contact.vue";
export default {
  layout: "servicesLayout",
  components: {
    About,
    About2,
    Services,
    Contact
  },
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
  }
};
</script>
