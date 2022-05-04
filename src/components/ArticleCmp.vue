<template>
  <article>
    <h2>{{ title }}</h2>
    <h2 v-bind="$attrs">Likes - {{ likes }}</h2>
    <h2>Published - {{ isPublished ? "Yes" : "No" }}</h2>
  </article>
</template>

<script>
export default {
  name: "ArticleCmp",
  props: {
    isPublished: {
      type: Boolean,
      required: true,
      default: false,
    },
    likes: {
      type: Number,
    },
    title: {
      type: String,
    },
  },
  inheritAttrs: false,
};
</script>

<style scoped>
</style>