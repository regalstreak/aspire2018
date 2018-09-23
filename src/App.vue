<template>
  <v-app>
    <v-toolbar
      app
      :clipped-left="clipped"
    >
      <v-toolbar-title><font style="font-family: 'Redressed; font-size: 2rem;'">{{title}}</font></v-toolbar-title>
    </v-toolbar>
    <v-content>
      <router-view/>
    </v-content>
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
      title: "aspire"
    };
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
