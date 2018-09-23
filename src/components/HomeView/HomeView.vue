<template>
  <v-layout column>
    <section>
      <v-parallax :src="`${baseUrl}parallax/hero.jpeg`" :height="windowHeight">

        <v-layout column align-center justify-center class="white--text">
          <img :src="`${baseUrl}parallax/vuetify.png`" alt="Vuetify.js" height="200">

          <h2 class="white--text mb-2 display-1 text-xs-center">
            <font class="itsa">
              ITSA
            </font>
          </h2>

          <div class="subheading mb-3 text-xs-center">
            <font class="mainhdr">
              Presents you with best events <br>
              Join the TechFest 2018
            </font>

          </div>

        </v-layout>
      </v-parallax>
    </section>

    <events />

    <past-numbers />

    <about />

  </v-layout>
</template>

<script>
import PastNumbers from "./contents/PastNumbers";
import Events from "./contents/Events";
import About from "./contents/About";

export default {
  components: {
    "past-numbers": PastNumbers,
    events: Events,
    about: About
  },
  computed: {
    baseUrl: () => {
      return process.env.BASE_URL;
    },
    windowHeight: () => {
      return window.innerHeight;
    }
  }
};
</script>

<style scoped>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

.itsa {
  font-family: "Redressed", cursive;
}

.mainhdr {
  font-family: "M PLUS Rounded 1c", sans-serif;
}
</style>
