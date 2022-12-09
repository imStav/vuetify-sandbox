<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>Lorem, ipsum dolor.</h3>
  </div>
</template>

<style scoped>
.greetings {
  display: flex;
  flex-direction: column;
}
</style>
