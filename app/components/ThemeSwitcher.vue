<script setup lang="ts">
const theme = useColorMode();

function change() {
  if (theme.preference == "light") {
    theme.preference = "dark";
  } else {
    theme.preference = "light";
  }
}
</script>

<template>
  <button @click="change">
    <Icon name="mdi:theme-light-dark" size="1.5rem" />
  </button>
</template>

<style lang="css" scoped>
button {
  display: contents;
}

button:hover {
  cursor: pointer;
}
</style>
