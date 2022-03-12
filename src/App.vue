<template>
  <v-app id="app">
    <app-bar />
    <v-main>
      <v-container>
        <router-view />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import AppBar from './components/AppBar.vue'

export default {
  components: {
    AppBar
  }
}
</script>

<style lang="scss">
#app {
  font-family: Roboto, sans-serif, Helvetica, Arial,;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

.container {
  max-width: 1200px !important;
}
</style>
