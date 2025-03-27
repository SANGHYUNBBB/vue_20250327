<script>
import Lesson1Parent from './lesson1/Lesson1Parent.vue'
export default {
  name: 'App',
  data() {
    return {}
  },
}
</script>

<template>
  <h1>컴포넌트 분리</h1>
  <lesson1Parent></lesson1Parent>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
