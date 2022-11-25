<script setup lang="ts">
import { ref } from "vue";

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
  <nav class="nav">
    <h1>{{msg}}</h1>
    <p>Last updated at: {{new Date().toString()}}</p>
  </nav>
</template>

<style scoped>
.nav  {
  text-align: center;
  padding: 2em;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  background-color: #fefefe;
}
.nav > p {
  font-size: 24px;
  font-weight: bold;
}
</style>
