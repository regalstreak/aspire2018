<template>
  <section>
    <v-parallax :src="`${baseUrl}parallax/section.jpg`" height="380">

      <v-container wrap>

        <v-flex class="text-xs-center">
          <div class="display-1 white--text mb-3 text-xs-center">
            Past Numbers
          </div>
          <br>

      <v-flex xs12>
        <v-container grid-list-xl>
          <v-layout row align-center>
          
            <v-flex xs6 lg3 mx-5>

              <v-card>
                <v-flex py-2>
                <v-icon x-large color="green darken-2">
                  business
                </v-icon>
                </v-flex>
                <v-flex pa-4>
                
                  <div class="display-3 text-xs-center">
                    {{4 * 100 / 5}}
                  </div>
                
                </v-flex>
                <v-flex py-1>
                
                  <div class="headline text-xs-center">
                    Events
                  </div>
                
                </v-flex>
                
              </v-card>
            </v-flex>
            <v-flex xs6 lg3 mx-5>

              <v-card>
                <v-flex py-2>
                <v-icon x-large color="green darken-2">
                  business
                </v-icon>
                </v-flex>
                <v-flex pa-4>
                
                  <div class="display-3 text-xs-center">
                    {{4 * 100 / 5}}
                  </div>
                
                </v-flex>
                <v-flex py-1>
                
                  <div class="headline text-xs-center">
                    Events
                  </div>
                
                </v-flex>
                
              </v-card>
            </v-flex>
            <v-flex xs12 lg3 mx-5>

              <v-card>
                <v-flex py-2>
                <v-icon x-large color="green darken-2">
                  business
                </v-icon>
                </v-flex>
                <v-flex pa-4>
                
                  <div class="display-3 text-xs-center">
                    {{4 * 100 / 5}}
                  </div>
                
                </v-flex>
                <v-flex py-1>
                
                  <div class="headline text-xs-center">
                    Events
                  </div>
                
                </v-flex>
                
              </v-card>
            </v-flex>
            <v-flex xs12 lg3 mx-5>

              <v-card>
                <v-flex py-2>
                <v-icon x-large color="green darken-2">
                  business
                </v-icon>
                </v-flex>
                <v-flex pa-4>
                
                  <div class="display-3 text-xs-center">
                    {{4 * 100 / 5}}
                  </div>
                
                </v-flex>
                <v-flex py-1>
                
                  <div class="headline text-xs-center">
                    Events
                  </div>
                
                </v-flex>
                
              </v-card>
            </v-flex>

          </v-layout>
        </v-container>
      </v-flex>


        </v-flex>

      </v-container>
    </v-parallax>
  </section>
</template>

<script>
export default {
  data: () => ({
    cards: {
      title: "Pre-fab homes",
      src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
      flex: 12
    }
  }),
  computed: {
    baseUrl: () => {
      return process.env.BASE_URL;
    }
  }
};
</script>

<style scoped>
.element {
  position: relative;
  top: 50%;
  transform: translateY(-50%);
  /* or try 50% */
}
</style>
