<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <!-- <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="@/assets/YoURL_logo.jpg"
          transition="scale-transition"
          width="40"
        /> -->
      </div>

      <v-spacer></v-spacer>

      <!-- <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      > -->
        <!-- <span class="mr-2">Latest Release</span> -->
        <!-- <v-icon>mdi-open-in-new</v-icon> -->
      <!-- </v-btn> -->
    </v-app-bar>

    <v-main>
      <urlShortener/>
    </v-main>
  </v-app>
</template>

<script>
import UrlShortener from '@/components/UrlShortener.vue'

export default {
  components: {
    UrlShortener
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
