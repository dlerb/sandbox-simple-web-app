<template>
  <!-- HTML-Element: h2 (titles) -->
  <h2 class="title">A simple Web App</h2>

  <!-- HTML-Element: div (container for misc things) -->
  <div class="cnt">Counter: {{ count }}</div>

  <!-- HTML-Element button -->
  <button class="btn" @click="handleAdd">Add 1</button>
</template>

<script setup>
import { ref } from "vue";
const count = ref(0);

// no-unused-vars
const handleAdd = () => {
  count.value = count.value + 1;
};
</script>

<style>
/* css styling for title */
h2 {
  color: royalblue;
  background-color: rgba(100, 100, 100, 0.1);
  padding: 5px;
  text-align: center;
}

/* css styling for counter */
.cnt {
  font-size: 22px;
  text-align: center;
  margin: auto;
}

/* css styling for button */
.btn {
  background-color: rgba(0, 0, 200, 0.1);
  border: 2px solid blue;
  border-radius: 5px;
  font-size: 15px;
  padding: 10px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-top: 15px;
}
</style>
