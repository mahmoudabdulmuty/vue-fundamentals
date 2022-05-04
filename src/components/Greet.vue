<template>
  <h2>
    Hello
    {{ username }} and age is {{ userAge }}
  </h2>
</template>

<script>
export default {
  name: "Greet",
  props: ["username", "userAge"],
};
</script>

<style scoped>
</style>