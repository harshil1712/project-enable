<template>
  <v-app id="inspire">
    <v-content>
      <v-container fluid fill-height>
        <v-layout align-center justify-center>
          <v-flex xs12 sm8 md4>
            <v-card class="elevation-12">
              <v-toolbar dark color="primary">
                <v-toolbar-title>Tutor SIGN UP FORM</v-toolbar-title>
                <v-spacer></v-spacer>
                <v-tooltip bottom>
                  <v-btn
                    slot="activator"
                    :href="source"
                    icon
                    large
                    target="_blank"
                  >

                  </v-btn>
                  <span>Source</span>
                </v-tooltip>
                <v-tooltip right>
                  <v-btn slot="activator" icon large href="https://codepen.io/johnjleider/pen/wyYVVj" target="_blank">
                    <v-icon large>mdi-codepen</v-icon>
                  </v-btn>
                  <span>Codepen</span>
                </v-tooltip>
              </v-toolbar>
              <v-card-text>
                <v-form>
                  <v-text-field prepend-icon="person" name="FULL NAME" label="FULL NAME" type="text"></v-text-field>
                  <v-text-field prepend-icon="build" name="Profession" label="Profession" type="text"></v-text-field>
                  <v-text-field prepend-icon="build" name="AreaOfInterest" label="Area Of Interest" type="text"></v-text-field>
                  <v-text-field prepend-icon="home" name="Address" label="Address" type="text"></v-text-field>
                  <v-text-field prepend-icon="history" name="AvailibilityTime" label="AvailibilityTime" type="text"></v-text-field>
                  <v-text-field prepend-icon="explicit" name="EMailId" label="E-Mail Id" type="text"></v-text-field>
                  <v-text-field prepend-icon="backup" name="Skype ID" label="Skype ID" type="text"></v-text-field>
                  <v-text-field id="password" prepend-icon="lock" name="password" label="Password" type="password"></v-text-field>
                </v-form>
              </v-card-text>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="primary">SUBMIT</v-btn>
              </v-card-actions>
            </v-card>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
  export default {
    data: () => ({
      drawer: null
    }),
    props: {
      source: String
    }
  }
</script>