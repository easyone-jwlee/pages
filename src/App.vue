<template>
  <v-app id="inspire">
    <app-bar />

    <v-main class="grey lighten-5">
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import AppBar from "./components/AppBar.vue";

export default {
  name: "App",
  components: {
    AppBar,
  },

  data: () => ({
    //
  }),
};
</script>
<style>
/*  
main color : #398860 
좀 더 진한 그린: #1a3134
제일 진한 그린: #244448
배경 연한 그린: #eff6f3
약간 노란 그린: #e5ead4



*/
</style>
