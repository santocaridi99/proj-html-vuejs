<template>
  <!-- sezione Dettagli -->
  <div class="container">
    <div class="detailsIntro">
      <p>MAXCOACH AVAILABLE COURSES</p>
      <h1>Access <span>Smart Tutoring</span> Program For Benefits.</h1>
    </div>
    <div class="datailscards">
      <div class="dcard">
        <div class="dcardimage">
          <img src="../assets/home-2-image-box-01.png" alt="home1" />
        </div>
        <div class="dcardText">
          <h1>Customize Preferences</h1>
          <p>
            Learners are given the right to arrange and customize their study
            schedule and timetable based on preferences.
          </p>
          <h4>Start Here &rarr;</h4>
        </div>
      </div>
      <div class="dcard">
        <div class="dcardimage">
          <img src="../assets/about-us-02-image-box-02.png" alt="home1" />
        </div>
        <div class="dcardText">
          <h1>Cloud Storage</h1>
          <p>
            You can store online lessons via online cloud or download to your
            device and revise lessons on the way.
          </p>
          <h4>Get Free Quote &rarr;</h4>
        </div>
      </div>
      <div class="dcard">
        <div class="dcardimage">
          <img src="../assets/home-2-image-box-03.png" alt="home3" />
        </div>
        <div class="dcardText">
          <h1>Multimedia Channels</h1>
          <p>
            We provide study materials with various formats: video,audio,slides,doc,prints,books and application
          </p>
          <h4>Start Now &rarr;</h4>
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
.container {
    margin-top: 80px;
  .detailsIntro {
    text-align: center;
    h1 {
      span {
        color: $TurquoiseBlue;
      }
    }
  }
  .datailscards {
    display: flex;
    margin-top: 50px;
    .dcard {
      width: calc(100% / 3 - 20px);
      margin: 20px;
    }
  }
}
</style>