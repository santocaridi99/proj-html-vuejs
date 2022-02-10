<template>
  <!-- dentro Headerbox inserirò tutto quello che ha a che fare con la navbar principale -->
  <header>
    <div class="container flex">
      <!-- qui ci sarà il logo con img -->
      <div class="logo flex">
        <img src="../assets/dark-logo.png" alt="MaxCoach" />
      </div>
      <!-- list div contenente una lista ul li dinamica -->
      <div class="list">
        <ul class="flex">
          <!-- per ogni link  presente nell'array di oggetti navbar -->
          <!-- stamperò un testo e un iconcina -->
          <li v-for="link in navbar" :key="link.id">
            <a :href="link.url">
              {{ link.text }}
            </a>
            <i class="fas fa-chevron-down"></i>
          </li>
        </ul>
      </div>
      <!-- sezione della user input -->
      <div class="userinput">
        <i class="far fa-user-circle"></i>
        <!-- qui inserisco la input -->
        <div class="inputbox flex">
          <input type="text" placeholder="Search.." />
          <i class="fas fa-search"></i>
        </div>
      </div>
    </div>
  </header>
</template>
<script>
export default {
  props: {
    //   passo dall'app l'array di oggetti navbar
    navbar: Array,
  },
};
</script>
<style lang="scss" scoped>
// importo scss
@import "@/style/variables.scss";
header {
  height: 80px;
  border-bottom: 5px solid $HintofRed;
  width: 100%;
  .container {
    height: 100%;
    align-items: center;
    justify-content: space-between;
    .logo {
      width: 160px;
      height: 50px;
      align-items: center;
      img {
        width: 100%;
      }
    }
    .list {
      ul {
        li {
          padding: 0 10px;
          a {
            color: $codGray;
          }
          // arrow verso il basso
          i {
            font-size: 10px;
          }
        }
      }
    }
    .userinput {
      display: flex;
      align-items: center;
      i {
        padding: 0 10px;
      }
      .fa-user-circle {
        font-size: 25px;
        margin-right: 20px;
      }
      .inputbox {
        background-color: $HintofRed;
        padding: 5px;
        height: 40px;
        align-items: center;
        border-radius: 5px;
        .fa-search {
          color: $MountainMeadow;
        }
      }
    }
  }
}
</style>