<template>
  <v-app>
    <v-main>

      <v-toolbar app class="warning">
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
        <v-toolbar-title>Vuetify</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn class="success ml-auto">
          Ingreso
        </v-btn>
        <v-btn class="error ml-auto">
          Salir
        </v-btn>
      </v-toolbar>

      <v-navigation-drawer app v-model="drawer" temporary dark>
        <v-layout mt-4 column align-center>
          <v-flex>
            <v-avatar>
              <v-img src="https://randomuser.me/api/portraits/men/85.jpg"></v-img>
            </v-avatar>
          </v-flex>
          <v-fle>
            <p class="white--text mt-3 headline">Juanito Perez</p>
          </v-fle>
        </v-layout>
      </v-navigation-drawer>
    </v-main>
  </v-app>
</template>

<script>


export default {
  name: 'App',
  data(){
    return{
      drawer: false
    }
  }
};
</script>
