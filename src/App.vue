<template>
  <card>
    <template v-slot:header>Card Content</template>
    <template v-slot:default>Card Default Content</template>
    <template v-slot:footer>
      <img src="https://picsum.photos/200" />
    </template>
  </card>
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