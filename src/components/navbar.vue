
<script setup>
import logo from '@/assets/images/logo.png'
</script>

<template>
    <nav class="bg-green-700 border-b border-green-500">
      <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
        <div class="flex h-20 items-center justify-between">
          <div
            class="flex flex-1 items-center justify-center md:items-stretch md:justify-start"
          ></div>
    <!-- Logo -->
            <a class="flex flex-shrink-0 items-center mr-4" href="index.html">
              <img class="h-10 w-auto" v-bind:src="logo" alt="Hashi cars" />
              <span class="hidden md:block text-white text-2xl font-bold ml-2"
                >Hashi cars</span
              >
            </a>
            <div class="md:ml-auto">
              <div class="flex space-x-2">
              </div>
            </div>
          </div>
        </div>
    </nav>
    <v-app-bar :elevation="3" color="beige" dark>
        <v-btn to="/"primary>Home</v-btn>
        <v-btn to="/browsecars">Browse cars</v-btn>
        <v-btn to="/sellyourcar">Sell your car</v-btn>
        <v-btn to="/aboutus">About us</v-btn>
        <v-btn to="/contactus">Contact us</v-btn>
    </v-app-bar>
</template>


