<script setup>
import Checkboxitem from './components/Checkboxitem4.vue';
import { ref } from 'vue';
</script>

<template>
  <h1>App 컴포넌트</h1>
  <hr />
  <Checkboxitem v-for="idol in idols" :key="idol.id" :idol="idol" />
</template>

<style scoped></style>
