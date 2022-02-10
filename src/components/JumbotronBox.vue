<template>
  <!--Jumbotron  -->
  <div class="container flex">
    <!-- area di testo jumbotron -->
    <div class="jumbotron-textarea">
      <h1>Distant Learning for further expansion</h1>
      <p>Learning is a life-long journey that in fact we never find</p>
      <p>the terminate stop.Stop searching,enjoy the process.</p>
      <button>
        <i class="fas fa-download"></i><span>Download free guide </span>
      </button>
      <p>
        Have questions?<span class="greenspan">Get Free Sample &rarr; </span>
      </p>
    </div>
    <!-- area immagine jumbo -->
    <div class="jumbotron-image">
      <img
        class="jumbo"
        src="../assets/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg"
        alt="jumbotron"
      />
      <img
        class="square layout"
        src="../assets/maxcoach-shape-08.png"
        alt="decoration1"
      />
      <img
        class="squaretwo layout"
        src="../assets/maxcoach-shape-08.png"
        alt="decoration2"
      />
      <img
        class="squarethree layout"
        src="../assets/maxcoach-shape-07.png"
        alt="decotation3"
      />
      <img
        class="layout-item layout"
        src="../assets/maxcoach-shape-02.png"
        alt="item2"
      />
      <img class="circle layout" src="../assets/screenshot.png" alt="decoration4" />
    </div>
    <!-- items del jumbotron -->
    <div class="jumbotron-items flex layout">
      <i class="fas fa-ruler-combined"></i>
      <i class="far fa-life-ring"></i>
      <i class="fas fa-book"></i>
      <i class="fas fa-shopping-cart"></i>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
// importo scss
@import "@/style/variables.scss";
.container {
  align-items: center;
  margin-top: 200px;
  justify-content: space-between;
  .jumbotron-textarea {
    width: 400px;
    p {
      font-weight: 400;
      span {
        font-weight: bolder;
        text-decoration: underline;
        text-decoration-color: $ShadyLady;
        cursor: pointer;
      }
    }
    button {
      span {
        margin-left: 5px;
      }
    }
  }
  .jumbotron-image {
    width: 650px;
    position: relative;
    .jumbo {
      border-radius: 50%;
      z-index: 1;
    }
    .square {
      left: -70px;
      top: 33%;
    }
    .squaretwo {
      left: -70px;
      top: 60%;
    }
    .squarethree {
      right: 40px;
      top: 60%;
    }
    .layout-item {
      top: 23%;
      right: -70px;
    }
    .circle{
      top:60%;
      left: -75px;
      z-index: -2;
    }
  }
  .jumbotron-items {
    right: 5px;
    height: 100px;
    align-self: flex-start;
    justify-content: space-between;
    flex-direction: column;
    box-shadow: 2px 2px 2px 2px $HintofRed;
  }
}
</style>