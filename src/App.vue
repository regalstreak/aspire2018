<template>
  <v-app>
    <v-toolbar
      app
      flat
      dense
      scroll-off-screen
      :color="updateToolbarScrollColor()"
      :scroll-threshold="70"
    >
      <v-toolbar-title><font style="font-family: 'Redressed; font-size: 2rem;'">{{title}}</font></v-toolbar-title>
    </v-toolbar>
      <router-view/>
    <v-footer >
      <v-layout column align-center>
        <pre><b>&lt;/&gt;</b> with <v-icon class="red--text" size="17">favorite</v-icon>️ by <b>Neil Agarwal</b></pre>
      </v-layout>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      title: "aspire",
      scrollPosition: null
    };
  },
  methods: {
    updateScroll() {
      this.scrollPosition = window.scrollY;
    },
    updateToolbarScrollColor() {
      if (this.scrollPosition >= 630) {
        return "undefined";
      } else {
        return "rgba(0, 0, 0, 0)";
      }
    }
  },
  mounted() {
    window.addEventListener("scroll", this.updateScroll);
  },
  destroy() {
    window.removeEventListener("scroll", this.updateScroll);
  }
};
</script>

<style scoped>
mainhdr {
  color: black;
  text-align: center;
  font-weight: bolder;
  font-size: 1rem;
  letter-spacing: 1px;
  overflow: auto;
  margin-top: 0px;
  padding: 0px;
  font-family: "M PLUS Rounded 1c", sans-serif;
}
</style>
