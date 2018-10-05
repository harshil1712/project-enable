<template>
  <v-form v-model="valid">
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
    
  </v-form>
   
</template>