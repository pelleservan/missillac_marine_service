<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <Header />
  <RouterView />
  <Footer />
</template>

<style scoped>
body,
html {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
