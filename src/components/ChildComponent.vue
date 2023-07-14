<template>
  <div class="">
    <div class="Hello">
      <h1>Hello, I am Child Component.</h1>
       <button @click="$emit('change-bg-red')">Change bg to red!</button>
    </div>

    <div class="message">
      <h2>{{ message }}</h2>
    </div>
    <slot name="changeBackgroundToRed" />
  </div>
</template>

<script setup>
import { ref, defineProps, defineEmits } from "vue";

const props = defineProps({
  message: String,
});

const emit = defineEmits(["change-bg-red"]);

</script>

<style scoped>
.message {
  background-color: rgb(173, 255, 221);
  height: 100px;
}
</style>
