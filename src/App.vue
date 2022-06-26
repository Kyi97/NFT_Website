<script setup>
import { RouterLink, RouterView } from "vue-router";
import NavBar from "./components/NavBar.vue";
</script>

<template>
  <header>
    <NavBar />
  </header>
  <RouterView />
</template>

<style>
@import "@/assets/base.css";
#app {
  margin: 0 auto;
  /* padding: 1rem 5rem 1rem 6rem; */
}
</style>
