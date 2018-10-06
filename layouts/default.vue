<template>
  <v-app light>
    <v-toolbar color="primary" 
      :fixed="fixed">
      <v-toolbar-title class="whiteColor">Project-ENABLE</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn flat nuxt to="/" color="white">Home</v-btn>
        <v-btn flat nuxt to="/about" color="white">About</v-btn>
        <v-btn flat nuxt to="/loginForm" color="white">Login</v-btn>
        <v-btn flat nuxt to="/signup" color="white">Sign Up</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-footer
      app
    >
    <span>&copy; 2017</span>
    </v-footer>
    <nuxt/>
  </v-app>

  
</template>

<style scoped>
.whiteColor{
  color: aliceblue;
}
</style>

<script>
  export default {
    data() {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'apps', title: 'Welcome', to: '/' },
          { icon: 'bubble_chart', title: 'Inspire', to: '/inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    }
  }
</script>
