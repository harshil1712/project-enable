<template>
  <v-container grid-list-md text-xs-center>
  <v-layout v-bind="binding">
  <v-layout row wrap>
  <v-flex md4 xs12>
    <nuxt-link to='inspire'>
        <v-card dark color="primary">
         <v-card-text><h1>Guardian</h1></v-card-text>
        </v-card>
    </nuxt-link>
  </v-flex>
    <v-flex md4 xs12>
      <nuxt-link to='inspire'>
        <v-card dark color="primary">
          <v-card-text><h1>Tutor</h1></v-card-text>
        </v-card>
      </nuxt-link>
      </v-flex>
     <v-flex md4 xs12>
      <nuxt-link  to='mentor'>
        <v-card dark color="primary">
         <v-card-text><h1>Mentor</h1></v-card-text>
        </v-card>
      </nuxt-link>
      </v-flex>
      </v-layout>
    </v-flex>
  </v-layout>
  </v-container>
</template>