<template>
  <card></card>
  <card>Card Content</card>
  <card><img src="https://picsum.photos/200" /></card>
</template>

<script>
import Card from "./components/Card";
export default {
  name: "App",
  components: {
    Card,
  },
};
</script>

<style scoped>
</style>