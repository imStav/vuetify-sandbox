<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <header>
    <HelloWorld msg="VuetifyIt!" />

    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  width: 70%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-block: 2rem;
  margin-inline: auto;
}

nav a {
  margin-inline: 0.5rem;
}

@media screen and (max-width: 700px) {
  header {
    width: 90%;
  }
}
</style>
