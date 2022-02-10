<template>
  <!-- sezione Dettagli o sezione About us-->
  <div class="container">
    <div class="detailsIntro">
      <p>MAXCOACH AVAILABLE COURSES</p>
      <h1>
        Access <span class="greenspan">Smart Tutoring</span> Program For
        Benefits.
      </h1>
    </div>
    <!-- tre card dove ci sono spiegati vari dettagli dell'azienda -->
    <!-- chiamate dcard, con sezione imagine , sezione testo -->
    <div class="datailscards flex">
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
            We provide study materials with various formats:
            video,audio,slides,doc,prints,books and application
          </p>
          <h4>Start Now &rarr;</h4>
        </div>
      </div>
    </div>
    <!-- sezione video -->
    <div class="media flex">
      <div class="video">
        <img src="../assets/home-2-popup-video-poster.jpg" alt="video" />
        <!-- icona youtube -->
        <img class="yt" src="../assets/icon-youtube-play.png" alt="youtube" />
        <!-- decorazioni -->
        <img class="layout shape" src="../assets/maxcoach-shape-05.png" alt="decoration">
        <img class="layout shape-second" src="../assets/maxcoach-shape-07.png" alt="decoration">
      </div>
      <div class="mediatext">
        <div class="subtitle">GET STARTED <strong>EFFORTLESSLY</strong></div>
        <h1>Enjoy Our</h1>
        <!-- scritta con grandezza e colore particolare -->
        <div><span class="companionship greenspan">Companionship</span></div>
        <p>
          Sneek peek into what has in store for you on our online teaching and
          mentoring portal.Seek for some hidden hints of early-bird rewards as
          well.
        </p>
        <!-- classe per link che porta a scaricare la guida(per ora un semplice div) -->
        <div class="freebook greenspan">Download free guidebook &rarr;</div>
      </div>
      <!-- decorazione -->
      <img
        class="circle"
        src="../assets/screenshot.png"
        alt="decoration"
      />
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
  }
  .datailscards {
    margin-top: 50px;
    .dcard {
      width: calc(100% / 3 - 20px);
      margin: 20px;
      h4 {
        cursor: pointer;
      }
    }
  }
  .media {
    position: relative;
    margin-top: 150px;
    justify-content: space-between;
    .video {
      position: relative;
      .yt {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
      }
      .shape{
        top:10%;
        left:-100px
      }
      .shape-second{
        bottom: -100px;
        right: -2%;
      }
    }
    .mediatext {
      width: 350px;
      .subtitle {
        color: $GunPowder;
        font-size: 14px;
      }
      h1 {
        font-size: 40px;
        margin-bottom: 10px;
      }
      .companionship {
        font-size: 40px;
      }
      .freebook {
        margin-top: 50px;
        font-weight: bolder;
        text-decoration: underline;
        cursor: pointer;
      }
    }
    .circle{
      position: absolute;
      top:-90px;
      left:58%;
    }
  }
}
</style>