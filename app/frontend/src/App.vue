<script setup lang="ts">
import { ref, onMounted } from "vue";

const message = ref("Loading...");

onMounted(async () => {
  const response = await fetch("http://localhost:9000");
  const data = await response.text();

  message.value = data;
})
</script>

<template>
  <p>Message from the backend: {{ message }}</p>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
