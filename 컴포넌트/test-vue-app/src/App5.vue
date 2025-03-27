<script setup>
import { ref } from 'vue';
const parentName = ref('');
</script>

<template>
  <h1>App 컴포넌트</h1>
  <hr />
  <div>
    <h3>App Data : {{ parentName }}</h3>
  </div>
</template>

<style scoped></style>
