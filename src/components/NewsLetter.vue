<template>
  <!-- sezione NewsLetter -->
  <div class="container">
    <div class="layout-item">
      <img src="../assets/screenshot2.png" alt="item" />
    </div>
    <div class="newsletter">
      <h1>Subscibe <span>Newsletters</span></h1>
      <p>Enter your email address to register to our newsletter subscription</p>
      <p>delivered on a regular basis!</p>
      <div class="inputbox">
        <div class="bg-hint">
          <input type="text" placeholder="Enter your email" />
        </div>
        <button>Subscibe</button>
      </div>
    </div>
    <div class="layout-item">
      <img src="../assets/maxcoach-shape-02.png" alt="item" />
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "@/style/variables.scss";
.container {
  padding: 80px;
  display: flex;
  justify-content: space-between;
  .newsletter {
    display: flex;
    flex-direction: column;
    text-align: center;
    h1 {
      span {
        color: $MountainMeadow;
      }
    }
    p {
      margin: 0;
    }
    .inputbox {
        margin-top: 50px;
      display: flex;
      .bg-hint {
        display: flex;
        input {
          width: 500px;
        }
      }
      button {
        margin: 0;
      }
    }
  }
}
</style>