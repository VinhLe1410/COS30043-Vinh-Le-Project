<script setup lang="ts">
import NavBar from './components/common/NavBar.vue'
import FooterBar from './components/common/FooterBar.vue'
</script>

<template>
  <div id="app">
    <NavBar />
    <router-view />
    <FooterBar />
  </div>
</template>
