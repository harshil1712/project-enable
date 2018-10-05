<template>

  <v-app dark>
    <v-toolbar>
      <v-toolbar-title>Project-ENABLE</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn flat>HOME</v-btn>
        <v-btn flat>CONTACT</v-btn>
        <v-btn flat>LOGIN</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-footer
      :fixed="fixed"
      app
    >
      <span>&copy; 2017</span>
    </v-footer>
    <nuxt/>
  </v-app>

  
</template>

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
