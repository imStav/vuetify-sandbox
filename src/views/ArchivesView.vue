<script setup>
import Alert from '../components/Alert.vue';
</script>

<template>
  <main>
    <h1>Archives</h1>

    <Alert status="info" message="This section regroups all archived articles, posts, cards." />
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
