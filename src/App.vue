<script setup>
import Navbar from "./components/navbar.vue"
</script>

<template>
  <v-app>
  <Navbar/>
  <v-main>
    <router-view></router-view>
  </v-main>
</v-app>
</template>
