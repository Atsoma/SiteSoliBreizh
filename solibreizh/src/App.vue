<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Header from "./components/Header.vue";

</script>

<template>
  <header>
      <Header />
  </header>
  <RouterView />
  <footer style="background-color: #0A72CC; color: white;">
    Numéro de telephone
    Réseaux Sociaux : 
    Facebook
    Linkedin
    Twitter
    Instagram
  </footer>
</template>

<style scoped>
  header{
    background-image: url(./assets/europraid-1.jpg);
    background-attachment: fixed;
  }

  body{
    font-family: Arial, Helvetica, sans-serif !important;
  }

</style>
