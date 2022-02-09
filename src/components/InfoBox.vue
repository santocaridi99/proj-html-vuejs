<template>
  <!-- sezione infobox -->
  <div class="infocontainer">
    <div class="container">
      <div class="infocard">
        <div class="icard">
          <h3>
            Successfully
            <div>trained</div>
          </h3>
          <!-- numero della carta -->
          <div class="icardnum">1720</div>
          <p>ENROLLED LEARNERS</p>
        </div>
        <div class="icard">
          <h3>
            Proudly
            <div>Received</div>
          </h3>
          <!-- numero della carta -->
          <div class="icardnum">19</div>
          <p>COUNTRYWIDE AWARDS</p>
        </div>
        <div class="icard">
          <h3>
            Firmly
            <div>Entstablished</div>
          </h3>
          <!-- numero della carta -->
          <div class="icardnum">24</div>
          <p>LOCAL BRANCHES</p>
        </div>
        <div class="icard">
          <h3>
            Getting
            <div>Featured on</div>
          </h3>
          <!-- numero della carta -->
          <div class="icardnum">1090</div>
          <p>BLOG POSTS</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "@/style/variables.scss";
.infocontainer {
  .container {
    .infocard {
      display: flex;
      justify-content: center;
      .icard {
        width: calc(100% / 4);
        padding: 30px;
        text-align: center;
        display: flex;
        flex-direction: column;
        justify-content: center;
        border: 2px solid $HintofRed;
        border-top: none;
        border-bottom: none;
        height: 300px;
        .icardnum {
          color: $MountainMeadow;
          font-weight: bold;
          font-size: 50px;
        }
      }
    }
  }
}
</style>