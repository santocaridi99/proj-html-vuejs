<template>
  <div id="app">
    <!-- sezione Header -->
    <header-box></header-box>
    <!-- sezione main  -->
    <main-content></main-content>
    <!-- sezione footer -->
    <footer-container></footer-container>
  </div>
</template>

<script>
// importo HeadeBox
import HeaderBox from './components/HeaderBox.vue'
// importo MainContent 
import MainContent from './components/MainContent.vue'
// importo FooterContainer
import FooterContainer from './components/FooterContainer.vue'

export default {
  name: 'App',
  // componenti principali
  components: {
    HeaderBox,
    MainContent,
    FooterContainer, 
  }
}
</script>

<style lang="scss">
// importo il main scss
@import './style/main.scss'
</style>
