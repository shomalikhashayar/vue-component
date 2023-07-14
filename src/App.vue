<template>
  <child-component
    @change-bg-red="changeBackgroundToRed"
    message="This is message comes from parrent...."
  >
    <template #changeBackgroundToRed>
     <H1>This template goes to child from parent by slots</H1>
    </template>
  </child-component>
</template>

<script setup>
import ChildComponent from "./components/ChildComponent.vue"

function changeBackgroundToRed() {
  document.body.style.background = 'red';
}
</script>

<style lang="scss" scoped></style>
