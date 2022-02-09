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
    <!-- sezione dei blog più visti -->
    <div class="bg-beige">
      <div class="container">
        <div class="blogcards">
          <div class="blog-text">
            <p>ENJOYABLE INSIGHTS</p>
            <h1>Most Viewed <span>Best Blogs</span></h1>
            <h5>&rarr; Become a Better Blogger:Content Planning</h5>
            <h5>&rarr; Promoting Your Online Business on Pinterest</h5>
            <h5>&rarr; Gamification and Game-Based Learning</h5>
            <h5>&rarr; Designing on Online Course from Expert's Perspective</h5>
            <h5>&rarr; Why Online Courses Are the Future of Education</h5>
          </div>
          <!-- blog card -->
          <div class="bcard">
            <div class="bimage">
              <img src="../assets/artist-blog-03-480x352.jpeg" alt="artist" />
            </div>
            <!-- testo della card degli artisti -->
            <div class="artistText">
              <p>ARTIST</p>
              <h4>Brush Strokes Energize Trees in Paintings</h4>
              <!-- sezione della card dove ci sono data e visualizzazioni -->
              <div class="date-views">
                <div class="date">
                  <i class="far fa-calendar-alt"></i>
                  <span>May 15,2020</span>
                </div>
                <div class="views">
                  <i class="far fa-eye"></i>
                  <span>688 views</span>
                </div>
              </div>
            </div>
          </div>
          <div class="bcard">
            <div class="bimage">
              <img src="../assets/artist-blog-01-480x352.jpg" alt="artist2" />
            </div>
            <!-- testo della card degli artisti -->
            <div class="artistText">
              <p>ARTIST</p>
              <h4>Pocket-Sized Notebooks Hold Miniature Pointings</h4>
              <!-- sezione della card dove ci sono data e visualizzazioni -->
              <div class="date-views">
                <div class="date">
                  <i class="far fa-calendar-alt"></i>
                  <span>May 15,2020</span>
                </div>
                <div class="views">
                  <i class="far fa-eye"></i>
                  <span>603 views</span>
                </div>
              </div>
            </div>
          </div>
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
  .bg-beige {
    background-color: $beige;
    padding: 100px;
    .container {
      .blogcards {
        display: flex;
        .blog-text {
            width: 50;
            align-self: center;
          h1 {
            span {
              color: $MountainMeadow;
            }
          }
        }
        .bcard {
            // width come se ci fossero tre card
          width: calc(100% / 3 - 70px);
          margin: 40px;
          .bimage {
            background-color: $white;
            img {
              width: 100%;
              height: 100%;
            }
          }
          .artistText {
            background-color: $white;
            padding: 40px;
            p {
              margin-top: 0;
            }
          }
          .date-views {
            color: $ShadyLady;
            font-size: 12px;
            display: flex;
            i{
                margin-right: 5px;
            }
            .views{
                margin-left: 20px;
            }
          }
        }
      }
    }
  }
}
</style>