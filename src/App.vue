<script setup>
import Navbar from "./components/navbar.vue"
import { RouterView } from 'vue-router';
</script>

<template>
  <Navbar/>
    <RouterView/>
</template>
<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100..900;1,100..900&display=swap");
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Roboto",sans-serif;
  font-weight: 400;
}
.app{
min-height: 100vh;
position: relative;
background-color: #f1f1f1;
}
.container{
  padding: 0 20px;
  max-width: 1140px;
  margin: 0 auto;
}
</style>