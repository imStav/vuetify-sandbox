<script setup>
import Card from "../components/Card.vue";
</script>

<template>
  <main>
    <div class="grid">
      <Card />
      <Card />
      <Card />
    </div>
  </main>
</template>

<style scoped>
main {
  width: 50%;
  margin-inline: auto;
}
.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
}

@media screen and (max-width: 1000px) {
  main {
    width: 70%;
  }
  .grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media screen and (max-width: 700px) {
  main {
    width: 90%;
  }
  .grid {
    grid-template-columns: repeat(1, 1fr);
  }
}

@media screen and (max-width: 500px) {
  main {
    width: 90%;
  }
  .grid {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>
