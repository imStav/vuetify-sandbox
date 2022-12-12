<script setup>
import { ref } from "vue";

const url = ref(
  "https://images.unsplash.com/photo-1620121684840-edffcfc4b878?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1632&q=80"
);

defineProps({
  title: {
    type: String,
    required: true,
  },
  description: {
    type: String,
    required: true,
  },
  author: {
    type: String,
    required: true,
  },
  date: {
    type: String,
    required: true,
  },
  status: {
    type: Boolean,
    required: true,
  }
});
</script>

<template>
  <v-card class="mx-auto rounded-lg elevation-0" variant="tonal" :color="status ? 'success' : 'warning'">
    <v-img class="align-end text-white" height="200" :src="url" cover>
      <v-card-title class="card_title">
        <h3>{{ title }}</h3>
      </v-card-title>
    </v-img>

    <v-card-subtitle class="card_subtitle pt-4">
      <p>{{ author }}</p>
      <span>|</span>
      <p>{{ date }}</p>
    </v-card-subtitle>

    <v-card-text>
      <p>{{ description }}</p>
    </v-card-text>

    <v-card-actions>
      <v-btn color="currentColor">
        <p v-if="status">Read more</p>
        <p v-else>Archived</p>
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

.card_subtitle {
  display: flex;
}

.card_subtitle span {
  margin-inline: .5rem;
}
</style>
