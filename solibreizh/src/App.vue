<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Header from "./components/Header.vue";

</script>

<template>
  <header>
      <Header />
  </header>
  <RouterView />
</template>

<style scoped>
  header{
    background-image: url(./assets/europraid-1.jpg);
    background-attachment: fixed;
  }
</style>
