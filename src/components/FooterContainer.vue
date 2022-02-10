<template>
  <footer>
    <div class="container">
      <!-- prima sezione del footer -->
      <div class="fFirst">
        <div class="address">
          <!-- per ogni oggetto presente nell'array address stampo il valore testo -->
          <h2>Address</h2>
          <p v-for="contact in address" :key="contact.id">{{ contact.text }}</p>
        </div>
        <!-- per ogni elemento presente nell'array assegno alla classe v-model il contenuto -->
        <div class="social">
          <i v-for="(social, i) in socials" :key="i" :class="social"></i>
        </div>
      </div>
      <!-- seconda sezione del footer -->
      <div class="fSecond">
        <div class="explore">
          <h2>Explore</h2>
          <ul class="flex">
            <!-- per ogni link presente nell'array links stampo il testo -->
            <li v-for="link in links" :key="link.id">
              <a :href="link.url">
                {{ link.text }}
              </a>
            </li>
          </ul>
        </div>
        <div class="rights">©2020 Maxcoach.All Rights Reserved</div>
      </div>
      <!-- terza sezione del footer -->
      <div class="fthird">
        <div class="information">
          <h2>Information</h2>
          <ul>
            <!-- per ogni informazione presente nell'array informations stampo testo -->
            <li v-for="info in informations" :key="info.id">
              <a :href="info.url">
                {{ info.text }}
              </a>
            </li>
          </ul>
        </div>
      </div>
      <!-- pulsante per tornare in cima -->
      <!-- click eseguiremo tramite il parent "top" -->
      <div class="backtop" @click="$emit('top')">
        <i class="fas fa-arrow-up"></i>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    // passo da app l'array di oggetti address
    address: Array,
    socials: Array,
    links: Array,
    informations: Array,
  },
};
</script>
<style lang="scss" scoped>
@import "@/style/variables.scss";
footer {
  background-color: $HintofRed;
  .container {
    position: relative;
    display: flex;
    padding: 80px;
    .fFirst,
    .fSecond,
    .fthird {
      width: calc(100% / 3 - 40px);
      margin: 40px;
    }
    .fFirst {
      .address {
        p {
          font-size: 14px;
        }
      }
      .social {
        margin-top: 50px;
        i {
          margin-right: 30px;
          font-size: 20px;
          color: $ShadyLady;
          cursor: pointer;
        }
      }
    }
    .fSecond {
      ul {
        flex-wrap: wrap;
        width: 220px;
        li {
          padding: 10px 10px;
        }
      }
      .rights {
        color: $ShadyLady;
        font-size: 14px;
        margin-top: 200px;
        margin-bottom: 0px;
      }
    }
    .fthird {
      .information {
        ul {
          padding-left: 0;
          li {
            padding: 10px 0;
          }
        }
      }
    }
    .backtop {
      position: absolute;
      bottom: 10%;
      right: 0;
      i {
        background-color: $MountainMeadow;
        color: $white;
        padding: 30px;
        border-radius: 50%;
        cursor: pointer;
      }
    }
  }
}
</style>