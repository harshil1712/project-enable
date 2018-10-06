<template>
  <v-app id="inspire">
    <v-content>
      <v-container fluid fill-height>
        <v-layout align-center justify-center>
          <v-flex xs12 sm8 md4>
            <v-card class="elevation-12">
              <v-toolbar dark color="primary">
                <v-toolbar-title>Login</v-toolbar-title>
                <v-spacer></v-spacer>
              </v-toolbar>
              <v-card-text>
                <v-form>
                  <v-text-field prepend-icon="person" name="email" label="Email ID" type="email" ref="emailInput" v-model="user.email" required></v-text-field>
                  <v-text-field id="password" prepend-icon="lock" name="password" label="Password" type="password" ref="passwordInput" v-model="user.password" required></v-text-field>
                </v-form>
              </v-card-text>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="primary" @click="submit()">Login</v-btn>
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
  data () {
    return {
      user: {
        email: '',
        password: ''
      }
    };
  },
  methods: {
    submit() {
      if(this.$refs.emailInput.value=='mentor' && this.$refs.passwordInput.value=='mentor'){
        this.$router.push("/")
      } else if(this.$refs.emailInput.value=='tutor' && this.$refs.passwordInput.value=='tutor'){
        this.$router.push("/")
      } else if(this.$refs.emailInput.value=='student' && this.$refs.passwordInput.value=='student'){
        this.$router.push("/studentdashboard")
      } else if(this.$refs.emailInput.value=='guardian' && this.$refs.passwordInput.value=='guardian'){
        this.$router.push("/")
      }
      console.log(this.email)
    }
  }
}
</script>
