<template>
  <h2>
    Cmp A
    {{ username }}
  </h2>
  <component-b />
</template>

<script>
import ComponentB from "./ComponentB.vue";
export default {
  components: { ComponentB },
  data() {
    return {
      username: "Mahmoud",
    };
  },
  provide() {
    return {
      name: this.username,
    };
  },
};
</script>

<style scoped>
</style>