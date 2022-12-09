<script setup>
import { ref } from "vue";
const url = ref(
  "https://images.unsplash.com/photo-1617457564031-cb8574d32ad8?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80"
);

const dateFrom = ref("01 Janvier 2023");
const dateTo = ref("01 Février 2023");
</script>

<template>
  <v-card class="mx-auto rounded-lg elevation-0" max-width="fit" color="info">
    <v-img class="align-end text-white" height="200" :src="url" cover>
      <v-card-title class="card_title">
        <h3>Lorem, ipsum dolor.</h3>
      </v-card-title>
    </v-img>

    <v-card-subtitle class="pt-4">
      <p>{{ dateFrom }} au {{ dateTo }}</p>
    </v-card-subtitle>

    <v-card-text>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae, suscipit?</p>
    </v-card-text>

    <v-card-actions>
      <v-btn color="white">
        <p>Action</p>
      </v-btn>

      <v-btn color="white">
        <p>Action</p>
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<style scoped>
.card_title {
  text-shadow: 1px 2px 3px black;
}
</style>
