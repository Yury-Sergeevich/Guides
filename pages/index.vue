<template>
  <div>
    <h2>Color mode: {{ $colorMode.value }}</h2>

    <Content />
  </div>
</template>

<script setup>
const colorMode = useColorMode();
definePageMeta({
  layout: "default",
});
</script>

<style lang="scss">
h1 {
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
}

body {
  background-color: #fff;
  color: rgba(0, 0, 0, 0.8);
}

.main {
  padding: 1em;
  overflow-y: hidden;
}
.dark-mode body {
  background-color: #202020;
  color: #ebf4f1;
}
.sepia-mode body {
  background-color: #f1e7d0;
  color: #433422;
}

.page-enter-active,
.page-leave-active {
  transition: all 0.4s;
}
.page-enter-from,
.page-leave-to {
  opacity: 0;
  filter: blur(1rem);
}
</style>
