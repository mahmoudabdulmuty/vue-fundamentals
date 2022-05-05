<template>
  <ul>
    <li v-for="username in usernames" :key="username.firstName">
      <slot
        :firstName="username.firstName"
        :lastName="username.lastName"
      ></slot>
    </li>
  </ul>
</template>

<script>
export default {
  name: "NameList",
  data() {
    return {
      usernames: [
        {
          firstName: "Mahmoud",
          lastName: "Abdulmuty",
        },
        {
          firstName: "Moemen",
          lastName: "Yasser",
        },
        {
          firstName: "John",
          lastName: "Snow",
        },
        {
          firstName: "Bruce",
          lastName: "Wayne",
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>