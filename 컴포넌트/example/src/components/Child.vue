<script setup>
import GrandChild from './GrandChild.vue';
</script>

<template>
  <div style="border: 2px solid yellow" class="child">
    <h1>나는 자식</h1>
    <GrandChild />
    <GrandChild /> <GrandChild />
  </div>
</template>

<style scoped></style>
