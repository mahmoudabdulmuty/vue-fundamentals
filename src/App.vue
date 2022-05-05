<template>
  <name-list>
    <template v-slot:default="slotProps">
      {{ slotProps.firstName }} {{ slotProps.lastName }}
    </template>
  </name-list>

  <name-list>
    <template v-slot:default="slotProps">
      {{ slotProps.lastName }} {{ slotProps.firstName }}
    </template>
  </name-list>
</template>

<script>
import NameList from "./components/NameList.vue";
export default {
  components: { NameList },
  name: "App",
};
</script>

<style scoped>
</style>