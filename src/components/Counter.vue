<script setup lang="ts">
import {computed, ref} from "vue";

  const counter = ref(0);
  const doubleCounter = computed(() => counter.value * 2);

  const increment = () => {
    counter.value++;
  }
  const decrement = () => {
    if (counter.value >= 1)
      counter.value--;
  }
</script>

<template>
  <h1>A - Counter</h1>
  <p>{{ counter }}</p>
  <p>Double counter: {{ doubleCounter }}</p>
  <p>
    <button @click="increment">Aufi</button>
    <button @click="decrement">Owi</button>
  </p>
</template>

<style scoped>

</style>