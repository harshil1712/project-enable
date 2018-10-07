<template>
  <v-container grid-list-md text-xs-center>
  <v-layout v-bind="binding" pt-5 mt-5>
  <v-layout row wrap pt-5 mt-5>
    
      <v-flex md4 xs12>
        <nuxt-link to='guardian'>
          <v-card dark color="primary">
            <v-card-text><h1>Guardian</h1></v-card-text>
              <v-card-text>
                <p class="text-xs-center"><h2>One who is the caretaker
                of the child and looks for the medium for the development
                of the child and also cooperates with the institution.</h2></p>
              </v-card-text>
          </v-card>
      </nuxt-link>
    </v-flex>
    <v-flex md4 xs12>
      <nuxt-link to='tutor'>
        <v-card dark color="primary">
          <v-card-text><h1>Tutor</h1></v-card-text>
          <v-card-text>
                <p class="text-xs-center"><h2>One who teches students through 
                video chat or personally as per conviniency and access the students
                on regular basis.</h2></p>
              </v-card-text>
        </v-card>
      </nuxt-link>
      </v-flex>
     <v-flex md4 xs12>
      <nuxt-link  to='mentor'>
        <v-card dark color="primary">
         <v-card-text><h1>Mentor</h1></v-card-text>
         <v-card-text>
                <p class="text-xs-center"><h2>One who manages and teaches the tutor and 
                  interacts with parents or guardians about 
                  the progress status of the student.</h2></p>
              </v-card-text>
        </v-card>
      </nuxt-link>
      </v-flex>
    
      </v-layout>
    
  </v-layout>
  </v-container>
</template>