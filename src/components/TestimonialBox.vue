<template>
  <!-- Sezione Testimonial  con le recensioni degli utenti -->
  <div class="testimonial-container">
    <div class="testimonial-title">
      <p>GREAT WORDS ABOUT MAXCOACH</p>
      <h1>Our <span>top learners' </span>verbatim</h1>
    </div>
    <!-- contenitore con card delle recensioni -->
    <div class="testimonial-cards">
      <div class="tcard opacity">
        <h3>High level of efficiency and scientific teaching methods</h3>
        <p>
          I am free to learn at my own pace,follow my own schedule and choose
          the subject I want to learn from the syllabus.Great study portal for
          people like me.
        </p>
        <div class="t-data">
          <img src="../assets/testimonial-avata-02.jpg" alt="testimonial1" />
          <div class="t-text">
            <h3>MINA HOLLACE</h3>
            <p>/ Freelance</p>
          </div>
        </div>
      </div>
      <div class="tcard">
        <h3>It's a choice of quality for people with special needs</h3>
        <p>
          I'm a very stict person so I require everything to be organized and
          neat.Then,I'll be able to make things right and shine.MaxCoach guys
          just got me.
        </p>
        <div class="t-data">
          <img src="../assets/testimonial-avata-03.jpg" alt="testimonial1" />
          <div class="t-text">
            <h3>Florenece Themes</h3>
            <p>/ Multimedia Admin</p>
          </div>
        </div>
      </div>
      <div class="tcard opacity">
        <h3>Professional team of specialist and passionate mentors at reach</h3>
        <p>
          I need to get a certification for English proficiency and MaxCoach is
          my best choice.Their tutors are smart and professional when dealing
          with students.
        </p>
        <div class="t-data">
          <img src="../assets/testimonial-avata-04.jpg" alt="testimonial1" />
          <div class="t-text">
            <h3>MADLEY PONDOR</h3>
            <p>/IT Specialist</p>
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="pallini">
          <div class="pallino pdark"></div>
          <div class="pallino"></div>
          <div class="pallino"></div>
          <div class="pallino"></div>
        </div>
      </div>
      <div class="row">
        <div class="layout-item fistItem">
          <img src="../assets/maxcoach-shape-01.png" alt="layout item" />
        </div>
        <!-- sezione di testo join con pulsante per iniziare i corsi -->
        <div class="join">
          <h3>Start today for getting <span>Online certification</span></h3>
          <h1>You can be your own guiding star with our help!</h1>
          <button>Get started now</button>
        </div>
        <div class="layout-item secondItem">
          <img src="../assets/maxcoach-shape-02.png" alt="layout item2" />
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
.testimonial-container {
  background-color: $HintofRed;
  margin-top: 80px;
  padding: 50px;
  .testimonial-title {
    text-align: center;
    h1 {
      span {
        color: $TurquoiseBlue;
      }
    }
  }
  .testimonial-cards {
    display: flex;
    .tcard {
      width: calc(100% / 3 - 20px);
      margin: 20px;
      padding: 20px;
      background-color: $white;
      .t-data {
        display: flex;
        margin-top: 50px;
        img {
          border-radius: 50%;
          width: 22%;
        }
        .t-text {
          margin-left: 20px;
          font-size: 12px;
        }
      }
    }
  }
  .container {
    .row {
      width: 100%;
      display: flex;
      justify-content: center;
      .pallini {
        display: flex;
        .pallino {
          margin: 50px 10px;
          width: 10px;
          height: 10px;
          background-color: lightgray;
          border-radius: 50%;
        }
        // pallino scuro
        .pdark {
          background-color: $GunPowder;
        }
      }
      .join {
        text-align: center;
        margin: 30px;
        h3 {
          margin-bottom: 5px;
          span {
            color: $TurquoiseBlue;
          }
        }
        h1 {
          margin-top: 0;
        }
      }
      .firstItem {
        align-self: center;
      }
      .secondItem {
        align-self: flex-end;
      }
    }
  }
}
</style>