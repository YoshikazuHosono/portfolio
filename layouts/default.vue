<template>
  <v-app>
    <v-app-bar elevation="4" dense app>
      <v-toolbar-title>Yoshikazu Hosono</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon @click="goTwitter">
        <v-icon>mdi-twitter</v-icon>
      </v-btn>
      <v-btn icon @click="goGithub">
        <v-icon>mdi-github</v-icon>
      </v-btn>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  methods: {
    goTwitter() {
      window.open("https://twitter.com/bb_kk_nn");
    },
    goGithub() {
      window.open("https://github.com/YoshikazuHosono");
    },
  },
};
</script>
