<template>
  <child-component message="This is message comes from parrent....">
    <template #changeBackgroundToRed>
      <button>Change bg to red!</button>
    </template>
  </child-component>
</template>

<script setup>
import ChildComponent from "./components/ChildComponent.vue";
</script>

<style lang="scss" scoped></style>
