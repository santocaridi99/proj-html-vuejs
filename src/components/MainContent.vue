<template>
  <div>
    <!-- sezione jumbotron -->
    <jumbotron-box></jumbotron-box>
    <!-- sezione partner aziendali -->
    <partner-box></partner-box>
    <!-- sezione corsi -->
    <courses-box></courses-box>
    <!-- sezione dettagli -->
    <details-box></details-box>
    <!-- sezione testimonial -->
    <testimonial-box></testimonial-box>
    <!-- sezione infobox -->
    <info-box></info-box>
    <!-- sezione NewsLetter -->
    <news-letter></news-letter>
  </div>
</template>
<script>
// importo jumbotron
import JumbotronBox from "./JumbotronBox.vue";
// importo partner box
import PartnerBox from "./PartnerBox.vue";
// importo CoursesBox
import CoursesBox from "./CoursesBox.vue";
// importo sezione dettagli
import DetailsBox from "./DetailsBox.vue";
// importo sezione testimonals
import TestimonialBox from "./TestimonialBox.vue";
// importo sezione info
import InfoBox from "./InfoBox.vue";
// importo sezione newsletter
import NewsLetter from "./NewsLetter.vue";

export default {
  components: {
    JumbotronBox,
    PartnerBox,
    CoursesBox,
    DetailsBox,
    TestimonialBox,
    InfoBox,
    NewsLetter,
  },
};
</script>
<style lang="scss" scoped>
@import "@/style/variables.scss";
</style>