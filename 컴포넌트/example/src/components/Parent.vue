<script setup>
import Child from './Child.vue';
import GrandChild from './GrandChild.vue';
</script>

<template>
  <div style="border: 5px solid blue" class="parent">
    <h1>나는 부모</h1>
    <Child /> <Child /> <GrandChild /> <GrandChild /> <GrandChild />
  </div>
</template>

<style scoped></style>
