<template>
  <div id="app">
    <!-- sezione Header -->
    <!-- props che passo all Header -->
    <header-box :navbar="navbar" :nlogo="logo"></header-box>
    <!-- sezione main  -->
    <main-content></main-content>
    <!-- sezione footer -->
    <!-- props che passo al footer -->
    <!-- al click di top eseguiremo funzione in methods scroll to top -->
    <footer-container
      :address="address"
      :socials="socials"
      :links="links"
      :informations="informations"
      @top="scrollToTop"
    ></footer-container>
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
      // oggetto con valore img che diamo valore require per farlo leggere
      // e msg che servirà per popolare l'alt
      logo: {
        img: require("./assets/dark-logo.png"),
        msg: "MaxCoach",
      },
      // array di oggetti per la navbar
      navbar: [
        {
          id: "1",
          text: "Home",
          dropone: "Infos",
          droptwo: "Our Story",
          droptree: "Join us",
        },
        {
          id: "2",
          text: "Pages",
          dropone: "Page1",
          droptwo: "Page 2",
          droptree: "Page 3",
        },
        {
          id: "3",
          text: "Courses",
          dropone: "Javascript",
          droptwo: "Artist",
          droptree: "Graphic",
        },
        {
          id: "4",
          text: "Features",
          dropone: "Features 1",
          droptwo: "Features2",
          droptree: "Features3",
        },
        {
          id: "5",
          text: "Blog",
          dropone: "Artist Blog",
          droptwo: "Best blogs",
          droptree: "EBlog",
        },
        {
          id: "6",
          text: "Shop",
          dropone: "Shop courses",
          droptwo: "Shop artist",
          droptree: "Shop gadget",
        },
      ],
      // array per indirizzi nel footer
      address: [
        {
          id: "7",
          text: "382 NE 191st St #87394 Miami,Fl 33179-3899",
          content: "address",
        },
        {
          id: "8",
          text: "+1(305)547-9909(9am - 5pm EST,Monday - Friday)",
          content: "number+disponibility",
        },
        {
          id: "9",
          text: "support@maxcoach.com",
          content: "email",
        },
      ],
      // array per icone social nel footer
      // usiamo fontawsome e passiamo i codici
      socials: [
        "fab fa-facebook-f",
        "fab fa-twitter",
        "fab fa-instagram",
        "fab fa-linkedin",
      ],
      // array per lista Explore nel footer
      links: [
        { id: "10", text: "Start Here", url: "/" },
        {
          id: "11",
          text: "Blog",
          url: "/",
        },
        {
          id: "12",
          text: "About us",
          url: "/",
        },
        {
          id: "13",
          text: "Success story",
          url: "/",
        },
        {
          id: "14",
          text: "Courses",
          url: "/",
        },
        {
          id: "15",
          text: "Contact us",
          url: "/",
        },
      ],
      // array informazioni nel footer
      informations: [
        {
          id: "16",
          text: "Membership",
          url: "/",
        },
        {
          id: "17",
          text: "Purchase guide",
          url: "/",
        },
        {
          id: "18",
          text: "Privacy policy",
          url: "/",
        },
        {
          id: "19",
          text: "Terms of services",
          url: "/",
        },
      ],
    };
  },
  methods: {
    // funzione che permette di tornare in cima alla finestra
    // con behavior smooth invece di farlo direttamente , lo esegue con animazione
    scrollToTop() {
      window.scrollTo({
        top: 0,
        left: 0,
        behavior: "smooth",
      });
    },
  },
};
</script>

<style lang="scss">
// importo il main scss
@import "./style/main.scss";
// import fontawesome
@import url("https://use.fontawesome.com/releases/v5.7.1/css/all.css");
</style>
