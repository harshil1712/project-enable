<template>
  <v-form ref="form" v-model="valid" lazy-validation>
    <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="20"
      label="Name"
      required
    ></v-text-field>

     <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="20"
      label="Child Name"
      required
    ></v-text-field>

     <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="20"
      label="Disability"
      required
    ></v-text-field>
     
     <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="20"
      label="Address"
      required
    ></v-text-field>

     <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="20"
      label="Learning Hours"
      required
    ></v-text-field>

     <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="20"
      label="Time Preference"
      required
    ></v-text-field>
    
    <v-text-field
      v-model="email"
      :rules="emailRules"
      label="E-mail"
      required
    ></v-text-field>
    
    
    
 
  <v-container grid-list-md>
    <v-layout row wrap>
      <v-flex xs12 lg6>
        <v-menu
          ref="menu1"
          :close-on-content-click="false"
          v-model="menu1"
          :nudge-right="40"
          lazy
          transition="scale-transition"
          offset-y
          full-width
          max-width="290px"
          min-width="290px"
        >
          <v-text-field
            slot="activator"
            v-model="dateFormatted"
            label="Date of child"
            hint="MM/DD/YYYY format"
            persistent-hint
            prepend-icon="event"
            @blur="date = parseDate(dateFormatted)"
          ></v-text-field>
          <v-date-picker v-model="date" no-title @input="menu1 = false"></v-date-picker>
        </v-menu>
        <p>Date in ISO format: <strong>{{ date }}</strong></p>
      </v-flex>
      </v-layout>
  </v-container>
   <v-text-field id="password" prepend-icon="lock" name="password" label="Password" type="password"></v-text-field>
  <v-checkbox
      v-model="checkbox"
      :rules="[v => !!v || 'You must agree to continue!']"
      label="Do you agree?"
      required
    ></v-checkbox>

    <v-btn
      :disabled="!valid"
      @click="submit"
    >
      submit
    </v-btn>
    <v-btn @click="clear">clear</v-btn>
   </v-form>
   
</template>