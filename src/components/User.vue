<template>
  <div class="hello">
    <h5>{{ msg }}</h5>

    <v-app id="e3" style="max-width: 400px; margin: auto;" standalone>
    <v-toolbar class="pink">
      <v-toolbar-side-icon></v-toolbar-side-icon>
      <v-toolbar-title class="white--text">My Music</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>search</v-icon>
      </v-btn>
    </v-toolbar>
    <main>
      <v-container
        fluid
        style="min-height: 0;"
        grid-list-lg
      >
        <v-layout row wrap>
          <v-flex xs12>
            <v-card class="blue-grey darken-2 white--text">
              <v-card-title primary-title>
                <div class="headline">Unlimited music now</div>
                <div>Listen to your favorite artists and albums whenenver and wherever, online and offline.</div>
              </v-card-title>
              <v-card-actions>
                <v-btn flat dark>Listen now</v-btn>
              </v-card-actions>
            </v-card>
          </v-flex>
          <v-flex xs12>
            <v-card class="cyan darken-2 white--text">
              <v-container fluid grid-list-lg>
                <v-layout row>
                  <v-flex xs7>
                    <div>
                      <div class="headline">Supermodel</div>
                      <div>Foster the People</div>
                    </div>
                  </v-flex>
                  <v-flex xs5>
                    <v-card-media
                      src="http://lorempixel.com/130/125/people/5/"
                      height="125px"
                      contain
                    ></v-card-media>
                  </v-flex>
                </v-layout>
              </v-container>
            </v-card>
          </v-flex>
          <v-flex xs12>
            <v-card class="purple white--text">
              <v-container fluid grid-list-lg>
                <v-layout row>
                  <v-flex xs7>
                    <div>
                      <div class="headline">Halycon Days</div>
                      <div>Ellie Goulding</div>
                    </div>
                  </v-flex>
                  <v-flex xs5>
                     <v-card-media
                        src="http://lorempixel.com/130/125/people/3/"
                        height="125px"
                        contain
                      ></v-card-media>
                  </v-flex>
                </v-layout>
              </v-container>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </main>
  </v-app>

    <app-userdetails></app-userdetails>
    <app-useredit></app-useredit>
    <hr>
    <button type="button" @click="show = true">Load Async component</button>
      <div v-if="show">
        <Async/>
  </div>

  </div>
</template>

<script>
import UserDetails from './UserDetails.vue'
import UserEdit from './UserEdit.vue'

export default {
  components: {
    appUserdetails: UserDetails,
    appUseredit: UserEdit
  },
  data () {
    return {
      msg: 'Welcome to App World',
      show: false
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
