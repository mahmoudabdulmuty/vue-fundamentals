<template>
  <custom-input v-model="username" />
</template>

<script>
import CustomInput from "./components/CustomInput.vue";
export default {
  data() {
    return {
      username: "",
    };
  },
  components: { CustomInput },
};
</script>

<style scoped>
</style>