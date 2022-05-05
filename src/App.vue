<template>
  <button @click="activeCMP = 'CmpA'">CMPA</button>
  <button @click="activeCMP = 'CmpB'">CMPB</button>
  <button @click="activeCMP = 'CmpC'">CMPC</button>
  <keep-alive>
    <component :is="activeCMP" />
  </keep-alive>
</template>

<script>
import CmpA from "./components/cmpA.vue";
import CmpB from "./components/cmpB.vue";
import CmpC from "./components/cmpC.vue";

export default {
  components: {
    CmpA,
    CmpB,
    CmpC,
  },
  name: "App",
  data() {
    return {
      activeCMP: "CmpA",
    };
  },
};
</script>

<style scoped>
</style>