<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >

      <h3 class="header">بنیاد برین</h3>
      <v-spacer></v-spacer>
      <div class="d-flex align-center">
        <h5>Barin Education</h5>
        <v-img
                alt="Vuetify Logo"
                class="shrink mr-2"
                contain
                :src="barin_logo"
                transition="scale-transition"
                width="70"
        />
      </div>
    </v-app-bar>
    <v-main style="font-family: Bnazanin,serif;">
      <info/>
      <search/>
      <BarinInfo />
    </v-main>
  </v-app>
</template>

<script>
import search from './components/search';
import info from './components/info';
import BarinInfo from "./components/BarinInfo";

export default {
  name: 'App',

  components: {
    search,
    info,
    BarinInfo
  },

  data: () => ({
    background_image: require('./assets/background.jpg'),
    barin_logo: require('./assets/barin-logo.png')
  }),
};
</script>
<style>
  @font-face {
    font-family: Bnazanin;
    src: url('assets/fonts/BNazanin.ttf');
  }
  @font-face {
    font-family: Bnazanin;
    src: url('assets/fonts/BNazanin.woff');
  }
  @font-face {
    font-family: Bnazanin;
    src: url('./assets/fonts/BNaznnBd.ttf');
  }
  .header {
    font-family: Bnazanin,serif;
    font-size: 20px;
  }
  #app {
      background: url('assets/background.jpg')
      no-repeat center center fixed !important;
      background-size: cover;
  }
</style>

