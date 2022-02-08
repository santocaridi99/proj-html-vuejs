<template>
  <div id="app">
    <!-- sezione Header -->
    <!-- navbar in Headerbox corrisponde al array in data di nome navbar -->
    <header-box :navbar="navbar"></header-box>
    <!-- sezione main  -->
    <main-content></main-content>
    <!-- sezione footer -->
    <footer-container></footer-container>
  </div>
</template>

<script>
// importo HeadeBox
import HeaderBox from "./components/HeaderBox.vue";
// importo MainContent
import MainContent from "./components/MainContent.vue";
// importo FooterContainer
import FooterContainer from "./components/FooterContainer.vue";

export default {
  name: "App",
  // componenti principali
  components: {
    HeaderBox,
    MainContent,
    FooterContainer,
  },
  data() {
    return {
      navbar:[
        {
          id:"1",
          text:"Home",
          url:"/"
        },
         {
          id:"2",
          text:"Pages",
          url:"/"
        },
         {
          id:"3",
          text:"Courses",
          url:"/"
        },
         {
          id:"4",
          text:"Features",
          url:"/"
        },
         {
          id:"5",
          text:"Blog",
          url:"/"
        },
         {
          id:"6",
          text:"Shop",
          url:"/"
        },

      ]
    };
  },
};
</script>

<style lang="scss">
// importo il main scss
@import "./style/main.scss";
// import fontawesome
@import url("https://use.fontawesome.com/releases/v5.7.1/css/all.css");
</style>
