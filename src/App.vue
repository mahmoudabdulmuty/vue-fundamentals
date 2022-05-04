<template>
  <h2>
    {{ counter }}
  </h2>
  <button @click="counter++">add by 1</button>
  <button @click="counter--">decrease by 1</button>
</template>

<script>
export default {
  data() {
    return { counter: 0 };
  },
  watch: {
    counter(newValue, oldValue) {
      if (newValue > oldValue && newValue === 16) {
        alert("counter is 16");
      }
    },
  },
};
</script>

<style>
</style>