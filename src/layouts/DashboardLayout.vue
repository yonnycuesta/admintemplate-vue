<template>
  <div>
     <v-toolbar color="primary">
      <v-toolbar-side-icon></v-toolbar-side-icon>
      <v-toolbar-title>Title</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn flat to="/register">Register</v-btn>
        <v-btn flat to="/login">Login</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-content>
    <slot></slot>
    </v-content>
    <v-footer
      height="auto"
      color="primary lighten-1"
    >
      <v-layout
        justify-center
        row
        wrap
      >
        <v-btn
          v-for="link in links"
          :key="link"
          color="white"
          flat
          round
        >
          {{ link }}
        </v-btn>
        <v-flex
          primary
          lighten-2
          py-3
          text-xs-center
          white--text
          xs12
        >
          &copy;2018 — <strong>Vuetify</strong>
        </v-flex>
      </v-layout>
    </v-footer>
  </div>
</template>
