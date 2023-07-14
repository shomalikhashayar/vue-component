<template>
  <div class="">
    <div class="Hello">
    <h1>Hello, I am Child Component.</h1>
  </div>

  <div class="message">
    <h2>{{ message }}</h2>
  </div>
  </div>
</template>

<script setup>
import { ref, defineProps } from "vue";

const props = defineProps({
  message: String,
});
</script>

<style scoped>
.message {
  background-color: rgb(173, 255, 221);
  height: 100px;
}
</style>
