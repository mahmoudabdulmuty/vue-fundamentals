<template>
  <button @click="isVisible = true">show</button>
  <popup v-show="isVisible" @close-modal="closeModal" />
</template>

<script>
import Popup from "./components/Popup.vue";
export default {
  name: "App",
  components: { Popup },
  data() {
    return {
      isVisible: false,
    };
  },
  methods: {
    closeModal() {
      this.isVisible = false;
    },
  },
};
</script>

<style scoped>
</style>