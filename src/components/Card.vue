<script setup>
import { ref } from "vue";
const url = ref(
  "https://images.unsplash.com/photo-1620121684840-edffcfc4b878?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1632&q=80"
);

const author = ref("imStav");
const date = ref("Feb. 1, 2023");
</script>

<template>
  <v-card class="mx-auto rounded-lg elevation-0" max-width="300" variant="tonal">
    <v-img class="align-end text-white" height="200" :src="url" cover>
      <v-card-title class="card_title">
        <h3>Lorem, ipsum dolor.</h3>
      </v-card-title>
    </v-img>

    <v-card-subtitle class="pt-4">
      <p>{{ author }} | {{ date }}</p>
    </v-card-subtitle>

    <v-card-text>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae, suscipit?</p>
    </v-card-text>

    <v-card-actions>
      <v-btn color="currentColor">
        <p>Read more</p>
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<style scoped>
.card_title {
  max-width: calc(300px - 2rem);
  text-shadow: 1px 2px 3px black;
  overflow: hidden;
  white-space: nowrap;
}

.card_title h3 {
  text-overflow: ellipsis;
}
</style>
