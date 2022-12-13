<script setup>
let blog = {
  name: 'Bloggy'
}
</script>

<template>
  <main class="about">
    <h1>About {{ blog.name }}</h1>
  </main>
</template>

<style scoped>
main {
  display: grid;
  max-width: 50%;
  margin-inline: auto;
  place-content: center;
  place-items: center;
}
</style>
