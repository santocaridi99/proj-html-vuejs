<template>
  <!-- sezione NewsLetter -->
  <div class="container flex">
    <div class="layout-item">
      <img src="../assets/screenshot2.png" alt="item" />
    </div>
    <div class="newsletter flex">
      <h1>Subscibe <span class="greenspan">Newsletters</span></h1>
      <p>Enter your email address to register to our newsletter subscription</p>
      <p>delivered on a regular basis!</p>
      <!-- sezione contentent input -->
      <div class="inputbox flex">
        <div class="bg-hint flex">
          <input type="text" placeholder="Enter your email" />
        </div>
        <button>Subscibe</button>
      </div>
    </div>
    <!-- item di layout -->
    <div class="layout-item">
      <img src="../assets/maxcoach-shape-02.png" alt="item" />
    </div>
    <!-- shape rotato  item di layout-->
    <img class="layout rshape" src="../assets/maxcoach-shape-09.png" alt="layout decoration">
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "@/style/variables.scss";
.container {
  margin-top: 60px;
  position: relative;
  padding: 80px;
  justify-content: space-between;
  .newsletter {
    flex-direction: column;
    text-align: center;
    p {
      margin: 0;
    }
    .inputbox {
      margin-top: 50px;
      .bg-hint {
        input {
          width: 500px;
        }
      }
      button {
        margin: 0;
      }
    }
  }
  .rshape{
    right: 100px;
    top: -50px;
  }
}
</style>