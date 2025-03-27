<script setup>
defineProps({
  id: [Number, String], // 문자열과 숫자열만 가능하다는 의미.
  name: String, // 문자만 받을 것이야
  checked: {
    type: Boolean, //불리언 타입만 가능
    default: false,
    required: true, // required 의 기본값은 트루임
  },
});
</script>
<!-- defineProps
 부모 컴포넌트에서 전달받은 프로퍼티를 정의하는 함수 -->

<template>
  <li><input type="checkbox" :checked="idol.checked" />{{ idol.name }}</li>
</template>

<style scoped></style>
