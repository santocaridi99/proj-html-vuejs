<template>
  <!-- dentro Headerbox inserirò tutto quello che ha a che fare con la navbar principale -->
  <header>
    <div class="container flex">
      <!-- qui ci sarà il logo con img -->
      <!-- nlogo sta per navbarlogo con valori img con url e msg alt -->
      <div class="logo flex">
        <img :src="nlogo.img" :alt="nlogo.msg" />
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
    // passo dall'app oggetto nlogo o navbarlogo
    nlogo:Object
  },
};
</script>
<style lang="scss" scoped>
// importo scss
@import "@/style/variables.scss";
header {
  height: 80px;
  width: 100%;
  background-color: $white;
  position: fixed;
  z-index: 1000;
  top: 0;
  border-bottom: 5px solid #f8f8f8;
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