<template>
  <div>
    <h2>Popup</h2>
    <input type="text" v-model="name" />
    <button @click="closeModal">close</button>
  </div>
</template>

<script>
export default {
  name: "Popup",
  data() {
    return {
      name: "",
    };
  },
  emits: {
    "close-modal"(name) {
      if (!name) {
        return false;
      }
      return true;
    },
  },
  methods: {
    closeModal() {
      this.$emit("close-modal", this.name);
    },
  },
};
</script>

<style scoped>
</style>