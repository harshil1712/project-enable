<template>
  <v-form ref="form" v-model="valid" lazy-validation>
    <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="10"
      label="Name"
      required
    ></v-text-field>
    <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="10"
      label="Profession"
      required
    ></v-text-field>
    <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="10"
      label="Area Of Interest"
      required
    ></v-text-field>
    <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="10"
      label="Availability"
      required
    ></v-text-field>
    <v-text-field
      v-model="email"
      :rules="emailRules"
      label="E-mail"
      required
    ></v-text-field>
    <v-text-field
      v-model="name"
      :rules="nameRules"
      :counter="10"
      label="Address"
      required
    ></v-text-field>
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