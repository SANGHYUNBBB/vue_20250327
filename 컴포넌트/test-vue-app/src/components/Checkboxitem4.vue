<script setup>
defineProps({
  idol: {
    // validator
    // vue 공식 기능
    // 부모가 prop을 전달할 때 마다 함수가 호출됨;
    type: Object,
    required: true,
    validator: (value) => {
      return (
        (typeof value.id === 'number' || typeof value.id === 'string') &&
        typeof value.name === 'string' &&
        typeof value.checked === 'boolean'
      );
    },
  },
});
</script>

<template>
  <li><input type="checkbox" :checked="idol.checked" />{{ idol.name }}</li>
</template>

<style scoped></style>
<!-- emit은 자식에서 발생한 이벤트를 전달해줌
 props은 요소 자체를 전달해주고!!!!!!! -->
