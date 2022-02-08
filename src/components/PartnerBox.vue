<template>
<!-- sezione dove inserisco tutti i loghi dei partner -->
  <div class="container">
    <div class="row">
      <div class="client">
        <img src="../assets/client-logo-01.png" alt="logo1" />
      </div>
      <div class="client">
        <img src="../assets/client-logo-02.png" alt="logo2" />
      </div>
      <div class="client">
        <img src="../assets/client-logo-03.png" alt="logo3" />
      </div>
      <div class="client">
        <img src="../assets/client-logo-04.png" alt="logo4" />
      </div>
      <div class="client">
        <img src="../assets/client-logo-05.png" alt="logo5" />
      </div>
      <div class="client">
        <img src="../assets/client-logo-06.png" alt="logo6" />
      </div>
      <div class="client">
        <img src="../assets/client-logo-07.png" alt="logo7" />
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.row {
  margin-top: 50px;
  display: flex;
  .client {
    width: calc(100% / 7 - 40px);
    margin: 40px;
    height: 80px;
    img {
      width: 100%;
      object-fit: cover;
    }
  }
}
</style>