<template>
  <v-app class="pink">
    <v-content class="">

      <v-container class="yellow">
        <v-layout column fill-height class="black">

          <v-flex class="orange white--text pa-1" sm12 width="100%">
            <h1>100 Vuetify Projects</h1>
          </v-flex> 

          <v-flex class="orange white--text pa-1" sm12>
            <h1>100 Vuetify Projects</h1>
          </v-flex>   

          <v-layout row wrap fill-height justify-center class="pa-3 ma-1 green">

            <v-flex class="" sm4 v-for="data in mock" v-bind:key="data.id" width="100%">
              <v-card class="ma-1">
                <v-card-title>
                  <h2>{{ data.name }}</h2>
                </v-card-title>
                <v-card-text>
                  <p>{{ data.desc }}</p>
                </v-card-text>
              </v-card>            
            </v-flex>  

          </v-layout>
           


        </v-layout>
      </v-container>

    </v-content>
  </v-app>
</template>

<script>

export default {
  name: 'App',
  components: {

  },
  data () {
    return {
      mock : [
        {id: 1234, name: "Leslie Tang", desc: "Not your average web dev"},
        {id: 65487, name: "Wonderweiss", desc: "A wonder whizz kid"},
        {id: 6854, name: "Conan Edogawa", desc: "Shonen Tantei"},
        {id: 8465, name: "Genta Kojima", desc: "Member of the Youth Detective Group"},
      ]
    }
  }
}
</script>
