<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <HelloWorld msg="You did it!" />

    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  width: 100%;
  display: flex;
  flex-direction: column;
  margin-block: 2rem;
}

nav {
  margin-inline: auto;
}
</style>
