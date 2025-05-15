<script setup lang="ts">
import NavBar from './components/common/NavBar.vue'
import FooterBar from './components/common/FooterBar.vue'
</script>

<template>
  <NavBar />
  <main class="container py-4">
    <router-view />
  </main>
  <FooterBar />
</template>

<style>
.container {
  min-height: calc(100vh - 180px); /* 100vh minus (navbar 80px + footer 100px) */
}
</style>
