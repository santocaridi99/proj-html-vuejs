<template>
  <!-- sezione Corsi -->
  <!-- dentro un container grande blu -->
  <div class="container-blue">
    <!-- container piccolo -->
    <div class="container">
      <!-- titolo della sezione coursetitle -->
      <div class="coursetitle">
        <p>STIMULATED TO LEARN?</p>
        <h1>Featured Online Courses</h1>
      </div>
      <div class="courses">
        <div class="course">
          <img src="../assets/course-02-480x298.jpg" alt="corso1" />
          <div class="coursetext">
            <div class="price">$40.00</div>
            <h3>Learning to Write as a Professional Author</h3>
            <div class="details">
              <i class="far fa-file-alt"></i>
              <span>20 lessons</span>
              <i class="far fa-user"></i>
              <span>50 Students</span>
            </div>
          </div>
        </div>
        <div class="course">
          <img src="../assets/stock-full-hd-03-480x298.jpg" alt="corso2" />
          <div class="coursetext">
            <div class="price">Free</div>
            <h3>Customer-centric Info-Tech Strategies</h3>
            <div class="details">
              <i class="far fa-file-alt"></i>
              <span>24 lessons</span>
              <i class="far fa-user"></i>
              <span>769 Students</span>
            </div>
          </div>
        </div>
        <div class="course">
          <img src="../assets/stock-full-hd-04-480x298.jpg" alt="corso3" />
          <div class="coursetext">
            <div class="price">$19.00</div>
            <h3>Open Programming Courses for Everyone: Python</h3>
            <div class="details">
              <i class="far fa-file-alt"></i>
              <span>17 lessons</span>
              <i class="far fa-user"></i>
              <span>62 Students</span>
            </div>
          </div>
        </div>
        <div class="course">
          <img src="../assets/stock-full-hd-06-480x298.jpg" alt="corso4" />
          <div class="coursetext">
            <div class="price">$40.00</div>
            <h3>Academic Listening and Note-taking</h3>
            <div class="details">
              <i class="far fa-file-alt"></i>
              <span>14 lessons</span>
              <i class="far fa-user"></i>
              <span>67 Students</span>
            </div>
          </div>
        </div>
        <div class="course">
          <img
            src="../assets/course-featured-image-01-480x298.jpg"
            alt="corso5"
          />
          <div class="coursetext">
            <div class="price">$39.00</div>
            <h3>Master jQuery in a Short Period of Time</h3>
            <div class="details">
              <i class="far fa-file-alt"></i>
              <span>6 lessons</span>
              <i class="far fa-user"></i>
              <span>51 Students</span>
            </div>
          </div>
        </div>
        <div class="course">
          <img src="../assets/stock-full-hd-05-480x298.jpg" alt="corso6" />
          <div class="coursetext">
            <div class="price">$59.00</div>
            <h3>Introducing to Javascript for Beginners</h3>
            <div class="details">
              <i class="far fa-file-alt"></i>
              <span>14 lessons</span>
              <i class="far fa-user"></i>
              <span>26 Students</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <button>View All courses &rarr;</button>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
@import "@/style/variables.scss";
.container-blue {
  background-color: $bgceleste;
  margin-top: 50px;
  .container {
    padding: 50px;
    .coursetitle {
      text-align: center;
    }
    .courses {
      display: flex;
      flex-wrap: wrap;
      .course {
        display: flex;
        width: calc(50% - 20px);
        margin-right: 20px;
        margin-top: 50px;

        img {
          width: 18%;
          border-radius: 50%;
          margin-right: 10px;
          object-fit: cover;
        }
        .details {
          font-size: 12px;
          color: $pcolor;
          i {
            padding: 0 10px;
          }
        }
      }
    }
  }
  .row {
    margin:30px 0;
    display: flex;
    justify-content: center;
    button{
      margin-bottom: 60px;
    }
  }
}
</style>