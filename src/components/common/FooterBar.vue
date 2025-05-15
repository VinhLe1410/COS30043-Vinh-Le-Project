<script setup lang="ts">
</script>

<template>
  <footer class="footer bg-dark text-light ">
    <div class="container">
      <h2>Contact Me</h2>
      <div class="contact-info">
        <p>Contact number: <a href="tel:+61433443221" class="text-light">0433 443 221</a></p>
        <p>Contact email: <a href="mailto:lpvinh2k4@gmail.com" class="text-light">lpvinh2k4@gmail.com</a></p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  position: fixed;
  bottom: 0;
  width: 100%;
}

.contact-info {
  margin-top: 1rem;
}

h2 {
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
}

a {
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}
</style>
