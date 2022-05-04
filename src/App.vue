<template>
  <greet username="Mahmoud" user-age="30" />
  <greet username="Mohamed" user-age="25" />
  <greet username="Ahmed" user-age="14" />
  <greet :username="channel" :user-age="userAge" />
  <article-cmp
    id="my-article"
    :title="channel"
    :isPublished="true"
    :likes="50"
  />
</template>

<script>
import ArticleCmp from "./components/ArticleCmp.vue";
import Greet from "./components/Greet.vue";

export default {
  name: "App",
  components: {
    Greet,
    ArticleCmp,
  },
  data() {
    return {
      channel: "CodeEvolution",
      userAge: 18,
    };
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>