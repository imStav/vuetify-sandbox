<script setup>
import Card from "../components/Card.vue";
</script>

<template>
  <main>
    <Card
      title="Lorem ipsum"
      description="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor."
      author="imStav"
      date="Feb. 1, 2023"
      :status="true"
    />
    <Card
      title="Lorem ipsum"
      description="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor."
      author="imStav"
      date="Feb. 1, 2023"
      :status="false"
    />
    <Card
      title="Lorem ipsum"
      description="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor."
      author="imStav"
      date="Feb. 1, 2023"
      :status="false"
    />
    <Card
      title="Lorem ipsum"
      description="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor."
      author="imStav"
      date="Feb. 1, 2023"
      :status="true"
    />
  </main>
</template>

<style scoped>
main {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
  max-width: 50%;
  margin-inline: auto;
  place-content: center;
  place-items: center;
}

@media screen and (max-width: 1650px) {
  main {
    max-width: 60%;
    grid-template-columns: repeat(2, 1fr);
  }
}

@media screen and (max-width: 1100px) {
  main {
    max-width: 70%;
  }
}

@media screen and (max-width: 950px) {
  main {
    max-width: 90%;
  }
}

@media screen and (max-width: 600px) {
  main {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>
