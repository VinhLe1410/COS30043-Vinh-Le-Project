<script setup lang="ts">
import { computed } from 'vue'
import { useRoute } from 'vue-router'

const route = useRoute()

const pageBranding = computed(() => {
  switch (route.name) {
    case 'home':
      return 'Home'
    case 'news':
      return 'News'
    case 'about':
      return 'About Us'
    default:
      return 'Home'
  }
})
</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark p-3">
    <span class="navbar-brand">{{ pageBranding }}</span>
    <button
      class="navbar-toggler"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#navbarNav"
      aria-controls="navbarNav"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item">
          <router-link class="nav-link" :class="{ active: route.name === 'home' }" to="/">Home</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" :class="{ active: route.name === 'news' }" to="/news">News</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" :class="{ active: route.name === 'about' }" to="/about">About</router-link>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
.router-link-active {
  font-weight: bold;
}

.navbar-brand {
  font-weight: normal;
}
</style>
