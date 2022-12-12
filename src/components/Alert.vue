<script setup>
defineProps({
  status: {
    type: String,
    required: true,
  },
  message: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <v-alert :color="status" variant="tonal" density="compact">
    {{ message }}
  </v-alert>
</template>
